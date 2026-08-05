---
title: Covariant Compositional Networks for Learning Graphs
arxiv_id: '1801.02144'
source_url: ''
authors:
- name: R. Kondor
  orcid: null
  s2_author_id: '2834541'
  s2_url: null
- name: H. Son
  orcid: null
  s2_author_id: '2125153550'
  s2_url: null
- name: Horace Pan
  orcid: null
  s2_author_id: '7823285'
  s2_url: null
- name: Brandon M. Anderson
  orcid: null
  s2_author_id: '2064907678'
  s2_url: null
- name: Shubhendu Trivedi
  orcid: null
  s2_author_id: '145927896'
  s2_url: null
published_date: Jan 7, 2018
published_date_iso: '2018-01-07'
published_venue: ICLR 2018
published_conference: ICLR 2018
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Most existing neural networks for learning graphs address permutation invariance
  by conceiving of the network as a message passing scheme, where each node sums the
  feature vectors coming from its neighbors. We argue that this imposes a limitation
  on their representation power, and instead propose a new general architecture for
  representing objects consisting of a hierarchy of parts, which we call covariant
  compositional networks (CCNs). Here, covariance means that the activation of each
  neuron must transform in a specific way under permutations, similarly to steerability
  in CNNs. We achieve covariance by making each activation transform according to
  a tensor representation of the permutation group, and derive the corresponding tensor
  aggregation rules that each neuron must implement. Experiments show that CCNs can
  outperform competing methods on standard graph learning benchmarks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Second order CCN
mrr: 0.0079
adjusted_mrr: 0.0053
mrr_dataset_count: 2
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: MUTAG
  rows:
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
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
    input_feature_source: null
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
  - model: ECC
    model_key: supcosine
    model_plain: ECC
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
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: cauemo
    model_plain: ECC
    value: 0.9692
    std: 0.0136
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.06283'
    title: 'Soft causal learning for generalized molecule property prediction: An
      environment modeling perspective'
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9692
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Second order CCN
    model_key: second order ccn
    model_plain: Second order CCN
    value: 0.9164
    std: 0.0724
    paper_value: 0.9164
    paper_std: 0.0724
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical description for kernel datasets
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9164
    true_std: 0.0724
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9164
    sort_std: 0.0724
    global_rank: 75
    paper_rank: 75
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.845
    std: 0.0216
    paper_value: 0.845
    paper_std: 0.0216
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical description for kernel datasets
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.86
    at_pub_std: 0.017
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2022-05-26'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.015000000000000013
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.904
    true_std: 0.057
    value_gap_source_arxiv: '2205.13328'
    value_gap_source_title: How Powerful are $K$-hop Message Passing Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.05900000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.057
    global_rank: 141
    paper_rank: 459
    rank_delta: 318
    rank_delta_abs: 318
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Neural graph fingerprints
    model_key: neural graph fingerprints
    model_plain: Neural graph fingerprints
    value: 0.89
    std: 0.07
    paper_value: 0.89
    paper_std: 0.07
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
    source_ref: Duvenaud2015
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical description for kernel datasets
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.89
    true_std: 0.07
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.89
    sort_std: 0.07
    global_rank: 256
    paper_rank: 256
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PSCN k=10
    model_key: pscn k=10
    model_plain: PSCN k=10
    value: 0.8895
    std: 0.0437
    paper_value: 0.8895
    paper_std: 0.0437
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
    source_ref: Niepert et al.
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical description for kernel datasets
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.8895
    at_pub_std: 0.0437
    at_pub_source_arxiv: '1605.05273'
    at_pub_source_title: Learning Convolutional Neural Networks for Graphs
    at_pub_source_date_iso: '2016-05-17'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2016-05-17'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8895
    true_std: 0.0437
    value_gap_source_arxiv: '1605.05273'
    value_gap_source_title: Learning Convolutional Neural Networks for Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8895
    sort_std: 0.0437
    global_rank: 259
    paper_rank: 259
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLG
    model_key: mlg
    model_plain: MLG
    value: 0.8794
    std: 0.0161
    paper_value: 0.8794
    paper_std: 0.0161
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical description for kernel datasets
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.8794
    at_pub_std: 0.0161
    at_pub_source_arxiv: '1603.06186'
    at_pub_source_title: The Multiscale Laplacian Graph Kernel
    at_pub_source_date_iso: '2016-03-01'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8794
    true_std: 0.0161
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8794
    sort_std: 0.0161
    global_rank: 311
    paper_rank: 311
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SP
    model_key: sp
    model_plain: SP
    value: 0.855
    std: 0.025
    paper_value: 0.855
    paper_std: 0.025
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical description for kernel datasets
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.858
    at_pub_std: 0.002
    at_pub_source_arxiv: '1410.3314'
    at_pub_source_title: Propagation Kernels
    at_pub_source_date_iso: '2014-10-13'
    at_pub_source_date_label: '2014'
    value_gap_source_date_iso: '2014-10-13'
    value_gap_source_date_label: '2014'
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.858
    true_std: 0.002
    value_gap_source_arxiv: '1410.3314'
    value_gap_source_title: Propagation Kernels
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.858
    sort_std: 0.002
    global_rank: 409
    paper_rank: 425
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL-Edge
    model_key: wl-edge
    model_plain: WL-Edge
    value: 0.8294
    std: 0.0233
    paper_value: 0.8294
    paper_std: 0.0233
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical description for kernel datasets
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.8294
    at_pub_std: 0.0233
    at_pub_source_arxiv: '1603.06186'
    at_pub_source_title: The Multiscale Laplacian Graph Kernel
    at_pub_source_date_iso: '2016-03-01'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8294
    true_std: 0.0233
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8294
    sort_std: 0.0233
    global_rank: 526
    paper_rank: 526
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.8244
    std: 0.0129
    paper_value: 0.8244
    paper_std: 0.0129
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical description for kernel datasets
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.8244
    at_pub_std: 0.0129
    at_pub_source_arxiv: '1603.06186'
    at_pub_source_title: The Multiscale Laplacian Graph Kernel
    at_pub_source_date_iso: '2016-03-01'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8244
    true_std: 0.0129
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8244
    sort_std: 0.0129
    global_rank: 552
    paper_rank: 552
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: p-RW
    model_key: p-rw
    model_plain: p-RW
    value: 0.8033
    std: 0.0135
    paper_value: 0.8033
    paper_std: 0.0135
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical description for kernel datasets
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8033
    true_std: 0.0135
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8033
    sort_std: 0.0135
    global_rank: 619
    paper_rank: 619
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
- &id002
  dataset: NCI1
  rows:
  - model: ECC
    model_key: wl-mlp
    model_plain: ECC
    value: 0.9954
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9954
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: gin
    model_plain: ECC
    value: 0.9934
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
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GNNs ... use node features
    is_global_top: true
    global_rank: 2
    sort_value: 0.9934
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ECC
    model_key: gcn
    model_plain: ECC
    value: 0.9727
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
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GNNs ... use node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.9727
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.8476
    std: 0.0032
    paper_value: 0.8476
    paper_std: 0.0032
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
    source_ref: Kriege16
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.859
    at_pub_std: 0.001
    at_pub_source_arxiv: '1410.3314'
    at_pub_source_title: Propagation Kernels
    at_pub_source_date_iso: '2014-10-13'
    at_pub_source_date_label: '2014'
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.011399999999999966
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86
    true_std: 0.018
    value_gap_source_arxiv: '2205.14368'
    value_gap_source_title: Going Deeper into Permutation-Sensitive Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.012399999999999967
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.018
    global_rank: 10
    paper_rank: 26
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Propagation Kernels
    comparison_source_arxiv: '1410.3314'
    is_best: false
    is_std_outlier: false
  - model: WL-Edge
    model_key: wl-edge
    model_plain: WL-Edge
    value: 0.8465
    std: 0.0025
    paper_value: 0.8465
    paper_std: 0.0025
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.8465
    at_pub_std: 0.0025
    at_pub_source_arxiv: '1603.06186'
    at_pub_source_title: The Multiscale Laplacian Graph Kernel
    at_pub_source_date_iso: '2016-03-01'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8465
    true_std: 0.0025
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8465
    sort_std: 0.0025
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLG
    model_key: mlg
    model_plain: MLG
    value: 0.8175
    std: 0.0024
    paper_value: 0.8175
    paper_std: 0.0024
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.8175
    at_pub_std: 0.0024
    at_pub_source_arxiv: '1603.06186'
    at_pub_source_title: The Multiscale Laplacian Graph Kernel
    at_pub_source_date_iso: '2016-03-01'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2018-05-21'
    value_gap_source_date_label: ICML 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8175
    true_std: 0.0024
    value_gap_source_arxiv: '1805.08090'
    value_gap_source_title: Graph Capsule Convolutional Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8175
    sort_std: 0.0024
    global_rank: 143
    paper_rank: 143
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PSCN k=10
    model_key: pscn k=10
    model_plain: PSCN k=10
    value: 0.7634
    std: 0.0168
    paper_value: 0.7634
    paper_std: 0.0168
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
    source_ref: Niepert et al.
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.7634
    at_pub_std: 0.0168
    at_pub_source_arxiv: '1605.05273'
    at_pub_source_title: Learning Convolutional Neural Networks for Graphs
    at_pub_source_date_iso: '2016-05-17'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2016-05-17'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7634
    true_std: 0.0168
    value_gap_source_arxiv: '1605.05273'
    value_gap_source_title: Learning Convolutional Neural Networks for Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7634
    sort_std: 0.0168
    global_rank: 402
    paper_rank: 402
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Second order CCN
    model_key: second order ccn
    model_plain: Second order CCN
    value: 0.7627
    std: 0.0413
    paper_value: 0.7627
    paper_std: 0.0413
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7627
    true_std: 0.0413
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7627
    sort_std: 0.0413
    global_rank: 405
    paper_rank: 405
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SP
    model_key: sp
    model_plain: SP
    value: 0.7361
    std: 0.0036
    paper_value: 0.7361
    paper_std: 0.0036
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.745
    at_pub_std: 0.003
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2016-06-03'
    value_gap_source_date_label: NeurIPS 2016
    gap_vs_at_pub: 0.008900000000000019
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.745
    true_std: 0.003
    value_gap_source_arxiv: '1606.01141'
    value_gap_source_title: On Valid Optimal Assignment Kernels and Applications to
      Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.008900000000000019
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.003
    global_rank: 443
    paper_rank: 464
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Valid Optimal Assignment Kernels and Applications
      to Graph Classification
    comparison_source_arxiv: '1606.01141'
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.624
    std: 0.0027
    paper_value: 0.624
    paper_std: 0.0027
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: 0.66
    at_pub_std: null
    at_pub_source_arxiv: '1603.05629'
    at_pub_source_title: Discriminative Embeddings of Latent Variable Models for Structured
      Data
    at_pub_source_date_iso: '2016-03-17'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2016-03-17'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: 0.03600000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.66
    true_std: null
    value_gap_source_arxiv: '1603.05629'
    value_gap_source_title: Discriminative Embeddings of Latent Variable Models for
      Structured Data
    value_gap_source_is_current_paper: false
    value_gap: 0.03600000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.66
    sort_std: null
    global_rank: 539
    paper_rank: 563
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Discriminative Embeddings of Latent Variable Models for
      Structured Data
    comparison_source_arxiv: '1603.05629'
    is_best: false
    is_std_outlier: false
  - model: Neural graph fingerprints
    model_key: neural graph fingerprints
    model_plain: Neural graph fingerprints
    value: 0.6221
    std: 0.0472
    paper_value: 0.6221
    paper_std: 0.0472
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
    source_ref: Duvenaud2015
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Jan 7, 2018
    date_display: Jan 2018
    date_iso: '2018-01-07'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6221
    true_std: 0.0472
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6221
    sort_std: 0.0472
    global_rank: 564
    paper_rank: 564
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
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: NCI1
      dataset_slug: nci1
single_proposed_model: Second order CCN
main_figure: /figures/1801.02144/main_figure.jpegoptim.jpg
---

