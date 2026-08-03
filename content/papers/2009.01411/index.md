---
title: Learning from Protein Structure with Geometric Vector Perceptrons
arxiv_id: '2009.01411'
source_url: ''
authors:
- name: Bowen Jing
  orcid: null
  s2_author_id: '2064253810'
  s2_url: null
- name: Stephan Eismann
  orcid: null
  s2_author_id: '2269018'
  s2_url: null
- name: Patricia Suriana
  orcid: null
  s2_author_id: '8844033'
  s2_url: null
- name: Raphael J. L. Townshend
  orcid: null
  s2_author_id: '144531620'
  s2_url: null
- name: R. Dror
  orcid: null
  s2_author_id: '2561280'
  s2_url: null
published_date: Sep 3, 2020
published_date_iso: '2020-09-03'
published_venue: ICLR 2020
published_conference: ICLR 2020
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'Learning on 3D structures of large biomolecules is emerging as a distinct
  area in machine learning, but there has yet to emerge a unifying network architecture
  that simultaneously leverages the geometric and relational aspects of the problem
  domain. To address this gap, we introduce geometric vector perceptrons, which extend
  standard dense layers to operate on collections of Euclidean vectors. Graph neural
  networks equipped with such layers are able to perform both geometric and relational
  reasoning on efficient representations of macromolecules. We demonstrate our approach
  on two important problems in learning from protein structure: model quality assessment
  and computational protein design. Our approach improves over existing classes of
  architectures on both problems, including state-of-the-art convolutional neural
  networks and graph neural networks. We release our code at.'
codebase_url: https://github.com/drorlab/gvp
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GVP-GNN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Power Flow Benchmarks
benchmark_coverage:
- benchmark: Power Flow Benchmarks
  benchmark_slug: power-flow-benchmarks
  evaluated: 1
  total: 2
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: Case 1
  rows:
  - model: GVP-GNN
    model_key: gvp-gnn
    model_plain: GVP-GNN
    value: 0.888
    std: null
    paper_value: 0.888
    paper_std: null
    metric: Pearson correlation
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Global Pearson correlation on 20 targets from CASP 13
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.888
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.888
    sort_std: null
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
  - model: ProQ3D
    model_key: proq3d
    model_plain: ProQ3D
    value: 0.847
    std: null
    paper_value: 0.847
    paper_std: null
    metric: Pearson correlation
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Global Pearson correlation on 20 targets from CASP 13
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.847
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.847
    sort_std: null
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SASHAN
    model_key: sashan
    model_plain: SASHAN
    value: 0.84
    std: null
    paper_value: 0.84
    paper_std: null
    metric: Pearson correlation
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
    table_ref: Table CASP 13
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Global Pearson correlation on 20 targets from CASP 13
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.84
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.84
    sort_std: null
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FaeNNz
    model_key: faennz
    model_plain: FaeNNz
    value: 0.81
    std: null
    paper_value: 0.81
    paper_std: null
    metric: Pearson correlation
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
    table_ref: Table CASP 13
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Global Pearson correlation on 20 targets from CASP 13
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.81
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.81
    sort_std: null
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphQA
    model_key: graphqa
    model_plain: GraphQA
    value: 0.81
    std: null
    paper_value: 0.81
    paper_std: null
    metric: Pearson correlation
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
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Stage 1 and Stage 2 Pearson correlation for CASP 12
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.81
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.81
    sort_std: null
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
  - model: VoroMQA-A
    model_key: voromqa-a
    model_plain: VoroMQA-A
    value: 0.744
    std: null
    paper_value: 0.744
    paper_std: null
    metric: Pearson correlation
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
    table_ref: Table CASP 13
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Global Pearson correlation on 20 targets from CASP 13
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.744
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.744
    sort_std: null
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
  - model: VoroMQA-B
    model_key: voromqa-b
    model_plain: VoroMQA-B
    value: 0.726
    std: null
    paper_value: 0.726
    paper_std: null
    metric: Pearson correlation
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
    table_ref: Table CASP 13
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Global Pearson correlation on 20 targets from CASP 13
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.726
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.726
    sort_std: null
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
  - model: ProQ4
    model_key: proq4
    model_plain: ProQ4
    value: 0.691
    std: null
    paper_value: 0.691
    paper_std: null
    metric: Pearson correlation
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
    table_ref: Table CASP 13
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Per-target Pearson correlation on 20 targets from CASP 13
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.691
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.691
    sort_std: null
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
  - model: Ornate
    model_key: ornate
    model_plain: Ornate
    value: 0.67
    std: null
    paper_value: 0.67
    paper_std: null
    metric: Pearson correlation
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
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Stage 1 and Stage 2 Pearson correlation for CASP 12
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.67
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.67
    sort_std: null
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
  - model: MULTICOM-NOVEL
    model_key: multicom-novel
    model_plain: MULTICOM-NOVEL
    value: 0.652
    std: null
    paper_value: 0.652
    paper_std: null
    metric: Pearson correlation
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
    table_ref: Table CASP 13
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Global Pearson correlation on 20 targets from CASP 13
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.652
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.652
    sort_std: null
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
  - model: SBROD
    model_key: sbrod
    model_plain: SBROD
    value: 0.64
    std: null
    paper_value: 0.64
    paper_std: null
    metric: Pearson correlation
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
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Stage 1 and Stage 2 Pearson correlation for CASP 12
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.64
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.64
    sort_std: null
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
  - model: 3DCNN
    model_key: 3dcnn
    model_plain: 3DCNN
    value: 0.61
    std: null
    paper_value: 0.61
    paper_std: null
    metric: Pearson correlation
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
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Stage 1 and Stage 2 Pearson correlation for CASP 12
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.61
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.61
    sort_std: null
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
  - model: VoroMQA
    model_key: voromqa
    model_plain: VoroMQA
    value: 0.61
    std: null
    paper_value: 0.61
    paper_std: null
    metric: Pearson correlation
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
    variant_inference_reason: 'dataset: fuzzy match to case 1 (score=77)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Stage 1 and Stage 2 Pearson correlation for CASP 12
    date: Sep 3, 2020
    date_display: Sep 2020
    date_iso: '2020-09-03'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-03'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.61
    true_std: null
    value_gap_source_arxiv: '2009.01411'
    value_gap_source_title: Learning from Protein Structure with Geometric Vector
      Perceptrons
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.61
    sort_std: null
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
  rank_metric: Pearson correlation
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Pearson correlation
  metric: Pearson correlation
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Power Flow Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Power Flow Benchmarks
    benchmark_slug: power-flow-benchmarks
    datasets:
    - dataset: Case 1
      dataset_slug: case-1
single_proposed_model: GVP-GNN
---

