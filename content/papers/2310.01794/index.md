---
title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based Gnn Explainers through
  In-depth Benchmarking'
arxiv_id: '2310.01794'
source_url: ''
authors:
- name: Mert Kosan
  orcid: null
  s2_author_id: '2134769449'
  s2_url: null
- name: S. Verma
  orcid: null
  s2_author_id: '143665702'
  s2_url: null
- name: Burouj Armgaan
  orcid: null
  s2_author_id: '2219690090'
  s2_url: null
- name: Khushbu Pahwa
  orcid: null
  s2_author_id: '1491635783'
  s2_url: null
- name: Ambuj K. Singh
  orcid: null
  s2_author_id: '2238534218'
  s2_url: null
- name: Sourav Medya
  orcid: null
  s2_author_id: '3390598'
  s2_url: null
- name: Sayan Ranu
  orcid: null
  s2_author_id: '2253455409'
  s2_url: null
published_date: Oct 3, 2023
published_date_iso: '2023-10-03'
published_venue: ICLR 2023
published_conference: ICLR 2023
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Numerous explainability methods have been proposed to shed light on the
  inner workings of Gnns. Despite the inclusion of empirical evaluations in all the
  proposed algorithms, the interrogative aspects of these evaluations lack diversity.
  As a result, various facets of explainability pertaining to Gnns, such as, their
  stability to variational factors such as different Gnn architectures, noise, stochasticity
  in non-convex loss surfaces, feasibility amidst domain constraints, and so forth,
  have yet to be formally investigated. Motivated by this need, we present a benchmarking
  study on perturbation-based explainability methods for Gnns, aiming to systematically
  evaluate and compare a wide range of explainability techniques. Among the key findings
  of our study, we identify the Pareto-optimal methods that exhibit superior efficacy
  and stability in the presence of noise. Nonetheless, our study reveals that all
  algorithms are affected by stability issues when faced with noisy data. Furthermore,
  we have established that the current generation of counterfactual explainers often
  fails to provide feasible recourses due to violations of topological constraints
  encoded by domain-specific considerations. Overall, this benchmarking study empowers
  stakeholders in the field of Gnns with a comprehensive understanding of the state-of-the-art
  explainability methods, potential research problems for further enhancement, and
  the implications of their application in real-world scenarios. =-1
codebase_url: https://github.com/Armagaan/gnn-x-bench
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
- TU Dortmund
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: MUTAG
  is_multi_metric: true
  rows:
  - model: RCExplainer
    model_key: rcexplainer
    model_plain: RCExplainer
    metric_values:
    - null
    - 0.4
    - 1.1
    - 0.94
    metric_stds:
    - null
    - 0.12
    - 0.22
    - 0.01
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.4
    sort_std: 0.12
    true_value: 0.4
    true_std: 0.12
    paper_value: 0.4
    paper_std: 0.12
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
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
    published_venue: ICLR 2023
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
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
  - model: CLEAR
    model_key: clear
    model_plain: CLEAR
    metric_values:
    - null
    - 0.55
    - 17.15
    - 0.88
    metric_stds:
    - null
    - 0.1
    - 1.62
    - 0.07
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.55
    sort_std: 0.1
    true_value: 0.55
    true_std: 0.1
    paper_value: 0.55
    paper_std: 0.1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
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
    published_venue: ICLR 2023
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 2
  - model: CF^2 (α=0)
    model_key: cf^2 (α=0)
    model_plain: CF^2 (α=0)
    metric_values:
    - null
    - 0.9
    - 1.0
    - null
    metric_stds:
    - null
    - 0.12
    - 0.0
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9
    sort_std: 0.12
    true_value: 0.9
    true_std: 0.12
    paper_value: 0.9
    paper_std: 0.12
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
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
    published_venue: ICLR 2023
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
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
  - model: CF^2
    model_key: cf^2
    model_plain: CF^2
    metric_values:
    - null
    - null
    - null
    - 0.94
    metric_stds:
    - null
    - null
    - null
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.94
    sort_std: 0.0
    true_value: 0.94
    true_std: 0.0
    paper_value: 0.94
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
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
    published_venue: ICLR 2023
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
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
  metrics:
  - Accuracy
  - Suffic.
  - Size
  - Sparsity
  primary_metric: Accuracy
  rank_metric: Suffic.
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Suffic.
  - Size
  - Sparsity
  metric: Suffic.
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id003
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8365
    std: 0.0201
    paper_value: 0.8365
    paper_std: 0.0201
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
    protocol_note: Test accuracy averaged over 10 runs with random seeds
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.9934
    at_pub_std: null
    at_pub_source_arxiv: '2202.10156'
    at_pub_source_title: 1-WL Expressiveness Is (Almost) All You Need
    at_pub_source_date_iso: '2022-02-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.15689999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9934
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.15689999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9934
    sort_std: null
    global_rank: 2
    paper_rank: 48
    rank_delta: 46
    rank_delta_abs: 46
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 1-WL Expressiveness Is (Almost) All You Need
    comparison_source_arxiv: '2202.10156'
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8243
    std: 0.028
    paper_value: 0.8243
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy averaged over 10 runs with random seeds
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.9727
    at_pub_std: null
    at_pub_source_arxiv: '2202.10156'
    at_pub_source_title: 1-WL Expressiveness Is (Almost) All You Need
    at_pub_source_date_iso: '2022-02-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.14839999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9727
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.14839999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9727
    sort_std: null
    global_rank: 3
    paper_rank: 107
    rank_delta: 104
    rank_delta_abs: 104
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 1-WL Expressiveness Is (Almost) All You Need
    comparison_source_arxiv: '2202.10156'
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8096
    std: 0.015
    paper_value: 0.8096
    paper_std: 0.015
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
    protocol_note: Test accuracy averaged over 10 runs with random seeds
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.9623
    at_pub_std: null
    at_pub_source_arxiv: '2202.10156'
    at_pub_source_title: 1-WL Expressiveness Is (Almost) All You Need
    at_pub_source_date_iso: '2022-02-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.15270000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9623
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.15270000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9623
    sort_std: null
    global_rank: 4
    paper_rank: 176
    rank_delta: 172
    rank_delta_abs: 172
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 1-WL Expressiveness Is (Almost) All You Need
    comparison_source_arxiv: '2202.10156'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8303
    std: 0.0137
    paper_value: 0.8303
    paper_std: 0.0137
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
    protocol_note: Test accuracy averaged over 10 runs with random seeds
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.82
    at_pub_std: 0.01
    at_pub_source_arxiv: '2201.13410'
    at_pub_source_title: 'Weisfeiler and Leman Go Infinite: Spectral and Combinatorial
      Pre-Colorings'
    at_pub_source_date_iso: '2022-01-31'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.010300000000000087
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8303
    true_std: 0.0137
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8303
    sort_std: 0.0137
    global_rank: 76
    paper_rank: 76
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
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
- &id001
  dataset: ogbg-molhiv
  is_multi_metric: true
  rows:
  - model: CF^2
    model_key: cf^2
    model_plain: CF^2
    metric_values:
    - null
    - null
    - null
    - 0.62
    metric_stds:
    - null
    - null
    - null
    - 0.05
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.62
    sort_std: 0.05
    true_value: 0.62
    true_std: 0.05
    paper_value: 0.62
    paper_std: 0.05
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
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
    published_venue: ICLR 2023
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
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
  - model: RCExplainer
    model_key: rcexplainer
    model_plain: RCExplainer
    metric_values:
    - null
    - 0.9
    - 1.0
    - 0.96
    metric_stds:
    - null
    - 0.02
    - 0.0
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.9
    sort_std: 0.02
    true_value: 0.9
    true_std: 0.02
    paper_value: 0.9
    paper_std: 0.02
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
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
    published_venue: ICLR 2023
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 1
  - model: CF^2 (α=0)
    model_key: cf^2 (α=0)
    model_plain: CF^2 (α=0)
    metric_values:
    - null
    - 0.96
    - 10.45
    - null
    metric_stds:
    - null
    - 0.0
    - 4.43
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.96
    sort_std: 0.0
    true_value: 0.96
    true_std: 0.0
    paper_value: 0.96
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
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
    published_venue: ICLR 2023
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
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
  metrics:
  - ROC-AUC
  - Suffic.
  - Size
  - Sparsity
  primary_metric: ROC-AUC
  rank_metric: Suffic.
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Suffic.
  - Size
  - Sparsity
  metric: Suffic.
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
- benchmark: TU Dortmund
  datasets:
  - *id002
  - *id003
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: NCI1
      dataset_slug: nci1
main_figure: /figures/2310.01794/main_figure.jpegoptim.jpg
---

