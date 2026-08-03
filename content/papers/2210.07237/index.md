---
title: 'Forces are not Enough: Benchmark and Critical Evaluation for Machine Learning
  Force Fields with Molecular Simulations'
arxiv_id: '2210.07237'
source_url: ''
authors:
- name: Xiang Fu
  orcid: null
  s2_author_id: '2119032930'
  s2_url: null
- name: Zhenghao Wu
  orcid: null
  s2_author_id: '1988569688'
  s2_url: null
- name: Wujie Wang
  orcid: null
  s2_author_id: '50976732'
  s2_url: null
- name: T. Xie
  orcid: null
  s2_author_id: '49902007'
  s2_url: null
- name: S. Keten
  orcid: null
  s2_author_id: '4886848'
  s2_url: null
- name: Rafael Gómez‐Bombarelli
  orcid: null
  s2_author_id: '1398336096'
  s2_url: null
- name: T. Jaakkola
  orcid: null
  s2_author_id: '35132120'
  s2_url: null
published_date: Oct 13, 2022
published_date_iso: '2022-10-13'
published_venue: TMLR 2022
published_conference: TMLR 2022
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: Molecular dynamics (MD) simulation techniques are widely used for various
  natural science applications. Increasingly, machine learning (ML) force field (FF)
  models begin to replace ab-initio simulations by predicting forces directly from
  atomic structures. Despite significant progress in this area, such techniques are
  primarily benchmarked by their force/energy prediction errors, even though the practical
  use case would be to produce realistic MD trajectories. We aim to fill this gap
  by introducing a novel benchmark suite for learned MD simulation. We curate representative
  MD systems, including water, organic molecules, peptide, and materials, and design
  evaluation metrics corresponding to the scientific objectives of respective systems.
  We benchmark a collection of state-of-the-art (SOTA) ML FF models and illustrate,
  in particular, how the commonly benchmarked force accuracy is not well aligned with
  relevant simulation metrics. We demonstrate when and how selected SOTA methods fail,
  along with offering directions for further improvement. Specifically, we identify
  stability as a key metric for ML models to improve. Our benchmark suite comes with
  a comprehensive open-source codebase for training and simulation with ML FFs to
  facilitate future work.
codebase_url: https://github.com/facebookresearch/fairchem
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Quantum Chemistry
benchmark_coverage:
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 1
  total: 3
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: MD17
  rows:
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
    value: 1.1
    std: null
    paper_value: 1.1
    paper_std: null
    metric: Force
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force MAE in meV/A on 10,000 randomly sampled test configurations
    date: Oct 13, 2022
    date_display: Oct 2022
    date_iso: '2022-10-13'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-13'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.1
    true_std: null
    value_gap_source_arxiv: '2210.07237'
    value_gap_source_title: 'Forces are not Enough: Benchmark and Critical Evaluation
      for Machine Learning Force Fields with Molecular Simulations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.1
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
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 1.5
    std: null
    paper_value: 1.5
    paper_std: null
    metric: Force
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force MAE in meV/A on 10,000 randomly sampled test configurations
    date: Oct 13, 2022
    date_display: Oct 2022
    date_iso: '2022-10-13'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-13'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.5
    true_std: null
    value_gap_source_arxiv: '2210.07237'
    value_gap_source_title: 'Forces are not Enough: Benchmark and Critical Evaluation
      for Machine Learning Force Fields with Molecular Simulations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.5
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
  - model: GemNet-T
    model_key: gemnet-t
    model_plain: GemNet-T
    value: 1.5
    std: null
    paper_value: 1.5
    paper_std: null
    metric: Force
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force MAE in meV/A on 10,000 randomly sampled test configurations
    date: Oct 13, 2022
    date_display: Oct 2022
    date_iso: '2022-10-13'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-13'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.5
    true_std: null
    value_gap_source_arxiv: '2210.07237'
    value_gap_source_title: 'Forces are not Enough: Benchmark and Critical Evaluation
      for Machine Learning Force Fields with Molecular Simulations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.5
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
  - model: GemNet-dT
    model_key: gemnet-dt
    model_plain: GemNet-dT
    value: 1.7
    std: null
    paper_value: 1.7
    paper_std: null
    metric: Force
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force MAE in meV/A on 10,000 randomly sampled test configurations
    date: Oct 13, 2022
    date_display: Oct 2022
    date_iso: '2022-10-13'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-13'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.7
    true_std: null
    value_gap_source_arxiv: '2210.07237'
    value_gap_source_title: 'Forces are not Enough: Benchmark and Critical Evaluation
      for Machine Learning Force Fields with Molecular Simulations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.7
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
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    value: 3.8
    std: null
    paper_value: 3.8
    paper_std: null
    metric: Force
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force MAE in meV/A on 10,000 randomly sampled test configurations
    date: Oct 13, 2022
    date_display: Oct 2022
    date_iso: '2022-10-13'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-13'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.8
    true_std: null
    value_gap_source_arxiv: '2210.07237'
    value_gap_source_title: 'Forces are not Enough: Benchmark and Critical Evaluation
      for Machine Learning Force Fields with Molecular Simulations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.8
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
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 4.2
    std: null
    paper_value: 4.2
    paper_std: null
    metric: Force
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force MAE in meV/A on 10,000 randomly sampled test configurations
    date: Oct 13, 2022
    date_display: Oct 2022
    date_iso: '2022-10-13'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-13'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 4.2
    true_std: null
    value_gap_source_arxiv: '2210.07237'
    value_gap_source_title: 'Forces are not Enough: Benchmark and Critical Evaluation
      for Machine Learning Force Fields with Molecular Simulations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 4.2
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
  - model: DeepPot-SE
    model_key: deeppot-se
    model_plain: DeepPot-SE
    value: 8.9
    std: null
    paper_value: 8.9
    paper_std: null
    metric: Force
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force MAE in meV/A on 10,000 randomly sampled test configurations
    date: Oct 13, 2022
    date_display: Oct 2022
    date_iso: '2022-10-13'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-13'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 8.9
    true_std: null
    value_gap_source_arxiv: '2210.07237'
    value_gap_source_title: 'Forces are not Enough: Benchmark and Critical Evaluation
      for Machine Learning Force Fields with Molecular Simulations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 8.9
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
  - model: ForceNet
    model_key: forcenet
    model_plain: ForceNet
    value: 9.9
    std: null
    paper_value: 9.9
    paper_std: null
    metric: Force
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force MAE in meV/A on 10,000 randomly sampled test configurations
    date: Oct 13, 2022
    date_display: Oct 2022
    date_iso: '2022-10-13'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-13'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 9.9
    true_std: null
    value_gap_source_arxiv: '2210.07237'
    value_gap_source_title: 'Forces are not Enough: Benchmark and Critical Evaluation
      for Machine Learning Force Fields with Molecular Simulations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 9.9
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
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 16.8
    std: null
    paper_value: 16.8
    paper_std: null
    metric: Force
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force MAE in meV/A on 10,000 randomly sampled test configurations
    date: Oct 13, 2022
    date_display: Oct 2022
    date_iso: '2022-10-13'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-13'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 16.8
    true_std: null
    value_gap_source_arxiv: '2210.07237'
    value_gap_source_title: 'Forces are not Enough: Benchmark and Critical Evaluation
      for Machine Learning Force Fields with Molecular Simulations'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 16.8
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
  rank_metric: Force
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - Force
  metric: Force
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Quantum Chemistry
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Quantum Chemistry
    benchmark_slug: quantum-chemistry
    datasets:
    - dataset: MD17
      dataset_slug: md17
---

