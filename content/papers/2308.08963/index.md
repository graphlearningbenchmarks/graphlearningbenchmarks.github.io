---
title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
arxiv_id: '2308.08963'
source_url: ''
authors:
- name: Xihong Yang
  orcid: null
  s2_author_id: '2154476091'
  s2_url: null
- name: Cheng Tan
  orcid: null
  s2_author_id: '2111728470'
  s2_url: null
- name: Yue Liu
  orcid: null
  s2_author_id: '2119034129'
  s2_url: null
- name: Ke Liang
  orcid: null
  s2_author_id: '2024445866'
  s2_url: null
- name: Siwei Wang
  orcid: null
  s2_author_id: '103307910'
  s2_url: null
- name: Sihang Zhou
  orcid: null
  s2_author_id: '2516087'
  s2_url: null
- name: Jun Xia
  orcid: null
  s2_author_id: '2069551655'
  s2_url: null
- name: Stan Z.Li
  orcid: null
  s2_author_id: '1390908654'
  s2_url: null
- name: Xinwang Liu
  orcid: null
  s2_author_id: '2130021053'
  s2_url: null
- name: En Zhu
  orcid: null
  s2_author_id: '2144622766'
  s2_url: null
published_date: Aug 17, 2023
published_date_iso: '2023-08-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Contrastive graph node clustering via learnable data augmentation is a hot
  research spot in the field of unsupervised graph learning. The existing methods
  learn the sampling distribution of a pre-defined augmentation to generate data-driven
  augmentations automatically. Although promising clustering performance has been
  achieved, we observe that these strategies still rely on pre-defined augmentations,
  the semantics of the augmented graph can easily drift. The reliability of the augmented
  view semantics for contrastive learning can not be guaranteed, thus limiting the
  model performance. To address these problems, we propose a novel CONtrastiVe Graph
  ClustEring network with Reliable AugmenTation (CONVERT). Specifically, in our method,
  the data augmentations are processed by the proposed reversible perturb-recover
  network. It distills reliable semantic information by recovering the perturbed latent
  embeddings. Moreover, to further guarantee the reliability of semantics, a novel
  semantic loss is presented to constrain the network via quantifying the perturbation
  and recovery. Lastly, a label-matching mechanism is designed to guide the model
  by clustering information through aligning the semantic labels and the selected
  high-confidence clustering pseudo labels. Extensive experimental results on seven
  datasets demonstrate the effectiveness of the proposed method. We release the code
  and appendix of CONVERT at https://github.com/xihongyang1999/CONVERT on GitHub.
codebase_url: https://github.com/xihongyang1999/CONVERT
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CONVERT
mrr: 0.4417
adjusted_mrr: 0.4417
mrr_dataset_count: 3
benchmark_categories:
- Hypergraph Benchmarks
benchmark_coverage:
- benchmark: Hypergraph Benchmarks
  benchmark_slug: hypergraph-benchmarks
  evaluated: 3
  total: 10
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: AMAP
  rows:
  - model: SCGDN
    model_key: idcrn
    model_plain: SCGDN
    value: 0.8208
    std: 0.0018
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_display: Feb 2022
    date_iso: '2022-02-25'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8208
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SCGDN
    model_key: dcrn
    model_plain: SCGDN
    value: 0.7966
    std: 0.0025
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_display: Feb 2022
    date_iso: '2022-02-25'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7966
    sort_std: 0.0025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SCGDN
    model_key: dfcn
    model_plain: SCGDN
    value: 0.76
    std: 0.008
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_display: Feb 2022
    date_iso: '2022-02-25'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.76
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CONVERT
    model_key: convert
    model_plain: CONVERT
    value: 0.7403
    std: 0.01
    paper_value: 0.7403
    paper_std: 0.01
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
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7403
    true_std: 0.01
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7403
    sort_std: 0.01
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
  - model: NACL
    model_key: nacl
    model_plain: NACL
    value: 0.7304
    std: 0.0108
    paper_value: 0.7304
    paper_std: 0.0108
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
    source_ref: AAAI 23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7304
    true_std: 0.0108
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7304
    sort_std: 0.0108
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AGE
    model_key: age
    model_plain: AGE
    value: 0.7174
    std: 0.0093
    paper_value: 0.7174
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
    source_ref: SIGKDD 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7174
    at_pub_std: 0.0093
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7174
    true_std: 0.0093
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7174
    sort_std: 0.0093
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    value: 0.7103
    std: 0.0064
    paper_value: 0.7103
    paper_std: 0.0064
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
    source_ref: IJCAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7103
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7103
    true_std: 0.0064
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7103
    sort_std: 0.0064
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
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.6999
    std: 0.0034
    paper_value: 0.6999
    paper_std: 0.0034
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
    source_ref: AAAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6999
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6999
    true_std: 0.0034
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6999
    sort_std: 0.0034
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.6987
    std: 0.0054
    paper_value: 0.6987
    paper_std: 0.0054
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
    source_ref: IJCAI 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6987
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6987
    true_std: 0.0054
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
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
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.5066
    std: 0.0149
    paper_value: 0.5066
    paper_std: 0.0149
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
    source_ref: WWW 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6805
    at_pub_std: 0.0181
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.17389999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6805
    true_std: 0.0181
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.17389999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6805
    sort_std: 0.0181
    global_rank: 17
    paper_rank: 32
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    value: 0.1597
    std: 0.0153
    paper_value: 0.1597
    paper_std: 0.0153
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
    source_ref: WWW 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1597
    at_pub_std: 0.0153
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.65
    true_std: 0.07
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.4903
    has_value_note: false
    value_note: ''
    sort_value: 0.65
    sort_std: 0.07
    global_rank: 20
    paper_rank: 39
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.643
    std: 0.0195
    paper_value: 0.643
    paper_std: 0.0195
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
    source_ref: TCYB 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6483
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.005299999999999971
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6483
    true_std: 0.0059
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.005299999999999971
    has_value_note: false
    value_note: ''
    sort_value: 0.6483
    sort_std: 0.0059
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    value: 0.5447
    std: 0.0083
    paper_value: 0.5447
    paper_std: 0.0083
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
    source_ref: ICLR 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6676
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.12290000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5447
    true_std: 0.0083
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5447
    sort_std: 0.0083
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.5359
    std: 0.0057
    paper_value: 0.5359
    paper_std: 0.0057
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
    source_ref: WWW 21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5359
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5359
    true_std: 0.0057
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5359
    sort_std: 0.0057
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.3288
    std: 0.055
    paper_value: 0.3288
    paper_std: 0.055
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
    source_ref: ICML 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated on AMAP dataset
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6283
    at_pub_std: 0.0159
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.2995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4273
    true_std: 0.0102
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.09850000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.4273
    sort_std: 0.0102
    global_rank: 35
    paper_rank: 37
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
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
- &id002
  dataset: BAT
  rows:
  - model: CONVERT
    model_key: convert
    model_plain: CONVERT
    value: 0.7777
    std: 0.0148
    paper_value: 0.7777
    paper_std: 0.0148
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
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7777
    true_std: 0.0148
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7777
    sort_std: 0.0148
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: K-means
    model_key: graphlearner
    model_plain: K-means
    value: 0.754
    std: 0.0088
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_display: Dec 2022
    date_iso: '2022-12-07'
    venue: ACM Multimedia
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.754
    sort_std: 0.0088
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: K-means
    model_key: scgdn
    model_plain: K-means
    value: 0.7449
    std: 0.0026
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    venue: ACM Multimedia
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7449
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.6702
    std: 0.0115
    paper_value: 0.6702
    paper_std: 0.0115
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
    source_ref: TCYB 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7174
    at_pub_std: 0.0093
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.04720000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7174
    true_std: 0.0093
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.04720000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7174
    sort_std: 0.0093
    global_rank: 5
    paper_rank: 11
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.4645
    std: 0.059
    paper_value: 0.4645
    paper_std: 0.059
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
    source_ref: WWW 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7125
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.248
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7125
    true_std: 0.0031
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.248
    has_value_note: false
    value_note: ''
    sort_value: 0.7125
    sort_std: 0.0031
    global_rank: 6
    paper_rank: 22
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: AGE
    model_key: age
    model_plain: AGE
    value: 0.5507
    std: 0.008
    paper_value: 0.5507
    paper_std: 0.008
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
    source_ref: SIGKDD 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7125
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.16180000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7125
    true_std: 0.0031
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.16180000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.7125
    sort_std: 0.0031
    global_rank: 7
    paper_rank: 12
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.2964
    std: 0.0049
    paper_value: 0.2964
    paper_std: 0.0049
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
    source_ref: ICML 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7047
    at_pub_std: 0.037
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.4083
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7047
    true_std: 0.037
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.4083
    has_value_note: false
    value_note: ''
    sort_value: 0.7047
    sort_std: 0.037
    global_rank: 8
    paper_rank: 30
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.5223
    std: 0.0003
    paper_value: 0.5223
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
    source_ref: IJCAI 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6987
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.1764
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6987
    true_std: 0.0054
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.1764
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
    global_rank: 9
    paper_rank: 15
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.5371
    std: 0.0034
    paper_value: 0.5371
    paper_std: 0.0034
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
    source_ref: WWW 21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5371
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5371
    true_std: 0.0034
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5371
    sort_std: 0.0034
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.4653
    std: 0.0057
    paper_value: 0.4653
    paper_std: 0.0057
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
    source_ref: AAAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4653
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4653
    true_std: 0.0057
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4653
    sort_std: 0.0057
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
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    value: 0.44
    std: 0.0062
    paper_value: 0.44
    paper_std: 0.0062
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
    source_ref: WWW 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.44
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.44
    true_std: 0.0062
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.44
    sort_std: 0.0062
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
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    value: 0.4233
    std: 0.0051
    paper_value: 0.4233
    paper_std: 0.0051
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
    source_ref: IJCAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4233
    at_pub_std: 0.0051
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4233
    true_std: 0.0051
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4233
    sort_std: 0.0051
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NACL
    model_key: nacl
    model_plain: NACL
    value: 0.4225
    std: 0.0034
    paper_value: 0.4225
    paper_std: 0.0034
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
    source_ref: AAAI 23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4225
    true_std: 0.0034
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4225
    sort_std: 0.0034
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    value: 0.3484
    std: 0.0015
    paper_value: 0.3484
    paper_std: 0.0015
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
    source_ref: ICLR 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via ten runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3484
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3484
    true_std: 0.0015
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3484
    sort_std: 0.0015
    global_rank: 30
    paper_rank: 30
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
- &id003
  dataset: EAT
  rows:
  - model: DFCN
    model_key: scagc
    model_plain: DFCN
    value: 0.7277
    std: 0.0016
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7277
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DFCN
    model_key: scgc
    model_plain: DFCN
    value: 0.7222
    std: 0.0097
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7222
    sort_std: 0.0097
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AGE
    model_key: age
    model_plain: AGE
    value: 0.4554
    std: 0.004
    paper_value: 0.4554
    paper_std: 0.004
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
    source_ref: SIGKDD 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7598
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.3044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7174
    true_std: 0.0093
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.262
    has_value_note: false
    value_note: ''
    sort_value: 0.7174
    sort_std: 0.0093
    global_rank: 3
    paper_rank: 20
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: true
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.3472
    std: 0.0016
    paper_value: 0.3472
    paper_std: 0.0016
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
    source_ref: IJCAI 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7596
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.41240000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6987
    true_std: 0.0054
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.3515
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
    global_rank: 5
    paper_rank: 25
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.5275
    std: 0.0007
    paper_value: 0.5275
    paper_std: 0.0007
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
    source_ref: TCYB 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6928
    at_pub_std: 0.023
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.1653
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.643
    true_std: 0.0195
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.11550000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.643
    sort_std: 0.0195
    global_rank: 7
    paper_rank: 11
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: CONVERT
    model_key: convert
    model_plain: CONVERT
    value: 0.5842
    std: 0.0022
    paper_value: 0.5842
    paper_std: 0.0022
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
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5842
    true_std: 0.0022
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5842
    sort_std: 0.0022
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
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.3342
    std: 0.031
    paper_value: 0.3342
    paper_std: 0.031
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
    source_ref: WWW 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5344
    at_pub_std: 0.0081
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.2002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5066
    true_std: 0.0149
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.17240000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.5066
    sort_std: 0.0149
    global_rank: 12
    paper_rank: 27
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.4822
    std: 0.0033
    paper_value: 0.4822
    paper_std: 0.0033
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
    source_ref: WWW 21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4822
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4822
    true_std: 0.0033
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4822
    sort_std: 0.0033
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.2535
    std: 0.0075
    paper_value: 0.2535
    paper_std: 0.0075
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
    source_ref: ICML 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4107
    at_pub_std: 0.0312
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.1572
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.47
    true_std: 0.06
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.21649999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.47
    sort_std: 0.06
    global_rank: 17
    paper_rank: 29
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    value: 0.3231
    std: 0.0097
    paper_value: 0.3231
    paper_std: 0.0097
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
    source_ref: WWW 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3231
    at_pub_std: 0.0097
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.42
    true_std: 0.06
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.09689999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.42
    sort_std: 0.06
    global_rank: 23
    paper_rank: 27
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    value: 0.352
    std: 0.0017
    paper_value: 0.352
    paper_std: 0.0017
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
    source_ref: IJCAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7681
    at_pub_std: 0.0145
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.4161
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.352
    true_std: 0.0017
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.352
    sort_std: 0.0017
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: NACL
    model_key: nacl
    model_plain: NACL
    value: 0.3125
    std: 0.0096
    paper_value: 0.3125
    paper_std: 0.0096
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
    source_ref: AAAI 23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3125
    true_std: 0.0096
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3125
    sort_std: 0.0096
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
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.3053
    std: 0.0147
    paper_value: 0.3053
    paper_std: 0.0147
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
    source_ref: AAAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4375
    at_pub_std: 0.0078
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.13219999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3053
    true_std: 0.0147
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3053
    sort_std: 0.0147
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    value: 0.2182
    std: 0.0098
    paper_value: 0.2182
    paper_std: 0.0098
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
    source_ref: ICLR 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance evaluated via 10 runs
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5455
    at_pub_std: 0.0097
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.3273
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2182
    true_std: 0.0098
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2182
    sort_std: 0.0098
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
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
- benchmark: Hypergraph Benchmarks
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Hypergraph Benchmarks
    benchmark_slug: hypergraph-benchmarks
    datasets:
    - dataset: AMAP
      dataset_slug: amap
    - dataset: BAT
      dataset_slug: bat
    - dataset: EAT
      dataset_slug: eat
single_proposed_model: CONVERT
---

