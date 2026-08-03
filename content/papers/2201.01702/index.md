---
title: 'Bringing Your Own View: Graph Contrastive Learning without Prefabricated Data
  Augmentations'
arxiv_id: '2201.01702'
source_url: ''
authors:
- name: Yuning You
  orcid: null
  s2_author_id: '89197162'
  s2_url: null
- name: Tianlong Chen
  orcid: null
  s2_author_id: '2034263179'
  s2_url: null
- name: Zhangyang Wang
  orcid: null
  s2_author_id: '2969311'
  s2_url: null
- name: Yang Shen
  orcid: null
  s2_author_id: '1705610299'
  s2_url: null
published_date: Jan 4, 2022
published_date_iso: '2022-01-04'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Self-supervision is recently surging at its new frontier of graph learning.
  It facilitates graph representations beneficial to downstream tasks; but its success
  could hinge on domain knowledge for handcraft or the often expensive trials and
  errors. Even its state-of-the-art representative, graph contrastive learning (GraphCL),
  is not completely free of those needs as GraphCL uses a prefabricated prior reflected
  by the ad-hoc manual selection of graph data augmentations. Our work aims at advancing
  GraphCL by answering the following questions: How to represent the space of graph
  augmented views? What principle can be relied upon to learn a prior in that space?
  And what framework can be constructed to learn the prior in tandem with contrastive
  learning? Accordingly, we have extended the prefabricated discrete prior in the
  augmentation set, to a learnable continuous prior in the parameter space of graph
  generators, assuming that graph priors per se, similar to the concept of image manifolds,
  can be learned by data generation. Furthermore, to form contrastive views without
  collapsing to trivial solutions due to the prior learnability, we have leveraged
  both principles of information minimization (InfoMin) and information bottleneck
  (InfoBN) to regularize the learned priors. Eventually, contrastive learning, InfoMin,
  and InfoBN are incorporated organically into one framework of bi-level optimization.
  Our principled and automated approach has proven to be competitive against the state-of-the-art
  graph self-supervision methods, including GraphCL, on benchmarks of small graphs;
  and shown even better generalizability on large-scale graphs, without resorting
  to human expertise or downstream validation. Our code is publicly released at.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LP
mrr: 0.0
adjusted_mrr: 0.0
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
  dataset: PPI
  rows:
  - model: LP
    model_key: pronet-all-atom
    model_plain: LP
    value: 0.871
    std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.12600'
    title: Learning Hierarchical Protein Representations via Complete 3D Graph Networks
    date: Jul 26, 2022
    date_display: Jul 2022
    date_iso: '2022-07-26'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/divelab/DIG
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.871
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LP
    model_key: gvp-gnn
    model_plain: LP
    value: 0.866
    std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.12600'
    title: Learning Hierarchical Protein Representations via Complete 3D Graph Networks
    date: Jul 26, 2022
    date_display: Jul 2022
    date_iso: '2022-07-26'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/divelab/DIG
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.866
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LP
    model_key: pronet-backbone
    model_plain: LP
    value: 0.858
    std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.12600'
    title: Learning Hierarchical Protein Representations via Complete 3D Graph Networks
    date: Jul 26, 2022
    date_display: Jul 2022
    date_iso: '2022-07-26'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/divelab/DIG
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.858
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LP-InfoBN
    model_key: lp-infobn
    model_plain: LP-InfoBN
    value: 0.7116
    std: 0.0028
    paper_value: 0.7116
    paper_std: 0.0028
    metric: AUROC
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transfer learning task on PPI dataset
    date: Jan 4, 2022
    date_display: Jan 2022
    date_iso: '2022-01-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7116
    true_std: 0.0028
    value_gap_source_arxiv: '2201.01702'
    value_gap_source_title: 'Bringing Your Own View: Graph Contrastive Learning without
      Prefabricated Data Augmentations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7116
    sort_std: 0.0028
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
  - model: LP
    model_key: lp
    model_plain: LP
    value: 0.701
    std: 0.0076
    paper_value: 0.701
    paper_std: 0.0076
    metric: AUROC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transfer learning task on PPI dataset
    date: Jan 4, 2022
    date_display: Jan 2022
    date_iso: '2022-01-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.701
    true_std: 0.0076
    value_gap_source_arxiv: '2201.01702'
    value_gap_source_title: 'Bringing Your Own View: Graph Contrastive Learning without
      Prefabricated Data Augmentations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.701
    sort_std: 0.0076
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
  - model: LP-InfoMin
    model_key: lp-infomin
    model_plain: LP-InfoMin
    value: 0.6824
    std: 0.0087
    paper_value: 0.6824
    paper_std: 0.0087
    metric: AUROC
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transfer learning task on PPI dataset
    date: Jan 4, 2022
    date_display: Jan 2022
    date_iso: '2022-01-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6824
    true_std: 0.0087
    value_gap_source_arxiv: '2201.01702'
    value_gap_source_title: 'Bringing Your Own View: Graph Contrastive Learning without
      Prefabricated Data Augmentations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6824
    sort_std: 0.0087
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.6788
    std: 0.0085
    paper_value: 0.6788
    paper_std: 0.0085
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: hu2019strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transfer learning task on PPI dataset as per hu2019strategies
    date: Jan 4, 2022
    date_display: Jan 2022
    date_iso: '2022-01-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6788
    true_std: 0.0085
    value_gap_source_arxiv: '2201.01702'
    value_gap_source_title: 'Bringing Your Own View: Graph Contrastive Learning without
      Prefabricated Data Augmentations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6788
    sort_std: 0.0085
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
  - model: EdgePred
    model_key: edgepred
    model_plain: EdgePred
    value: 0.657
    std: 0.013
    paper_value: 0.657
    paper_std: 0.013
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: hu2019strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transfer learning task on PPI dataset as per hu2019strategies
    date: Jan 4, 2022
    date_display: Jan 2022
    date_iso: '2022-01-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.657
    true_std: 0.013
    value_gap_source_arxiv: '2201.01702'
    value_gap_source_title: 'Bringing Your Own View: Graph Contrastive Learning without
      Prefabricated Data Augmentations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.657
    sort_std: 0.013
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
  - model: AttrMasking
    model_key: attrmasking
    model_plain: AttrMasking
    value: 0.652
    std: 0.016
    paper_value: 0.652
    paper_std: 0.016
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: hu2019strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transfer learning task on PPI dataset as per hu2019strategies
    date: Jan 4, 2022
    date_display: Jan 2022
    date_iso: '2022-01-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.652
    true_std: 0.016
    value_gap_source_arxiv: '2201.01702'
    value_gap_source_title: 'Bringing Your Own View: Graph Contrastive Learning without
      Prefabricated Data Augmentations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.652
    sort_std: 0.016
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
  - model: No pre-train.
    model_key: no pre-train.
    model_plain: No pre-train.
    value: 0.648
    std: 0.01
    paper_value: 0.648
    paper_std: 0.01
    metric: AUROC
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
    table_ref: Table 4
    source_ref: hu2019strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transfer learning task on PPI dataset as per hu2019strategies
    date: Jan 4, 2022
    date_display: Jan 2022
    date_iso: '2022-01-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.648
    true_std: 0.01
    value_gap_source_arxiv: '2201.01702'
    value_gap_source_title: 'Bringing Your Own View: Graph Contrastive Learning without
      Prefabricated Data Augmentations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.648
    sort_std: 0.01
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
  - model: ContextPred
    model_key: contextpred
    model_plain: ContextPred
    value: 0.644
    std: 0.013
    paper_value: 0.644
    paper_std: 0.013
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: hu2019strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transfer learning task on PPI dataset as per hu2019strategies
    date: Jan 4, 2022
    date_display: Jan 2022
    date_iso: '2022-01-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.644
    true_std: 0.013
    value_gap_source_arxiv: '2201.01702'
    value_gap_source_title: 'Bringing Your Own View: Graph Contrastive Learning without
      Prefabricated Data Augmentations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.644
    sort_std: 0.013
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
  - model: Infomax
    model_key: infomax
    model_plain: Infomax
    value: 0.641
    std: 0.015
    paper_value: 0.641
    paper_std: 0.015
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: hu2019strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transfer learning task on PPI dataset as per hu2019strategies
    date: Jan 4, 2022
    date_display: Jan 2022
    date_iso: '2022-01-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.641
    true_std: 0.015
    value_gap_source_arxiv: '2201.01702'
    value_gap_source_title: 'Bringing Your Own View: Graph Contrastive Learning without
      Prefabricated Data Augmentations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.641
    sort_std: 0.015
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AUROC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - AUROC
  metric: AUROC
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
    - dataset: PPI
      dataset_slug: ppi
single_proposed_model: LP
---

