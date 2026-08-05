---
title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical Analysis of GNN
  Explanation Methods'
arxiv_id: '2106.09078'
source_url: ''
authors:
- name: Chirag Agarwal
  orcid: null
  s2_author_id: '40228633'
  s2_url: null
- name: M. Zitnik
  orcid: null
  s2_author_id: '2095762'
  s2_url: null
- name: Himabindu Lakkaraju
  orcid: null
  s2_author_id: '1892673'
  s2_url: null
published_date: Jun 16, 2021
published_date_iso: '2021-06-16'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: As Graph Neural Networks (GNNs) are increasingly being employed in critical
  real-world applications, several methods have been proposed in recent literature
  to explain the predictions of these models. However, there has been little to no
  work on systematically analyzing the reliability of these methods. Here, we introduce
  the first-ever theoretical analysis of the reliability of state-of-the-art GNN explanation
  methods. More specifically, we theoretically analyze the behavior of various state-of-the-art
  GNN explanation methods with respect to several desirable properties (e.g., faithfulness,
  stability, and fairness preservation) and establish upper bounds on the violation
  of these properties. We also empirically validate our theoretical results using
  extensive experimentation with nine real-world graph datasets. Our empirical results
  further shed light on several interesting insights about the behavior of state-of-the-art
  GNN explanation methods.
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
- TU Dortmund
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 2
  total: 16
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id001
  dataset: CiteSeer
  is_multi_metric: true
  rows:
  - model: GraphLIME
    model_key: graphlime
    model_plain: GraphLIME
    metric_values:
    - null
    - 0.001
    - 0.048
    metric_stds:
    - null
    - 0.0
    - 0.015
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.001
    sort_std: 0.0
    true_value: 0.001
    true_std: 0.0
    paper_value: 0.001
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Random Node Features
    model_key: random node features
    model_plain: Random Node Features
    metric_values:
    - null
    - 0.003
    - 0.18
    metric_stds:
    - null
    - 0.0
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.003
    sort_std: 0.0
    true_value: 0.003
    true_std: 0.0
    paper_value: 0.003
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: VanillaGrad
    model_key: vanillagrad
    model_plain: VanillaGrad
    metric_values:
    - null
    - 0.003
    - 0.142
    metric_stds:
    - null
    - 0.0
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.003
    sort_std: 0.0
    true_value: 0.003
    true_std: 0.0
    paper_value: 0.003
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    metric_values:
    - null
    - 0.003
    - 0.212
    metric_stds:
    - null
    - 0.0
    - 0.015
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.003
    sort_std: 0.0
    true_value: 0.003
    true_std: 0.0
    paper_value: 0.003
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Integrated Gradients
    model_key: integrated gradients
    model_plain: Integrated Gradients
    metric_values:
    - null
    - 0.004
    - 0.896
    metric_stds:
    - null
    - 0.0
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.004
    sort_std: 0.0
    true_value: 0.004
    true_std: 0.0
    paper_value: 0.004
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Random Edges
    model_key: random edges
    model_plain: Random Edges
    metric_values:
    - null
    - 0.005
    - 0.263
    metric_stds:
    - null
    - 0.0
    - 0.019
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.005
    sort_std: 0.0
    true_value: 0.005
    true_std: 0.0
    paper_value: 0.005
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: PGMExplainer
    model_key: pgmexplainer
    model_plain: PGMExplainer
    metric_values:
    - null
    - 0.009
    - 0.262
    metric_stds:
    - null
    - 0.001
    - 0.015
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.009
    sort_std: 0.001
    true_value: 0.009
    true_std: 0.001
    paper_value: 0.009
    paper_std: 0.001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: PGExplainer
    model_key: pgexplainer
    model_plain: PGExplainer
    metric_values:
    - null
    - 0.129
    - 0.4
    metric_stds:
    - null
    - 0.01
    - 0.017
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.129
    sort_std: 0.01
    true_value: 0.129
    true_std: 0.01
    paper_value: 0.129
    paper_std: 0.01
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: GraphMask
    model_key: graphmask
    model_plain: GraphMask
    metric_values:
    - null
    - 0.17
    - 0.2
    metric_stds:
    - null
    - 0.007
    - 0.028
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.17
    sort_std: 0.007
    true_value: 0.17
    true_std: 0.007
    paper_value: 0.17
    paper_std: 0.007
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 9
  metrics:
  - Accuracy
  - Unfaithfulness
  - Instability
  primary_metric: Accuracy
  rank_metric: Unfaithfulness
  higher_is_better: false
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Unfaithfulness
  - Instability
  metric: Unfaithfulness
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id005
  dataset: MUTAG
  is_multi_metric: true
  rows:
  - model: Random Edges
    model_key: random edges
    model_plain: Random Edges
    metric_values:
    - null
    - 0.022
    - 0.366
    metric_stds:
    - null
    - 0.029
    - 0.064
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.022
    sort_std: 0.029
    true_value: 0.022
    true_std: 0.029
    paper_value: 0.022
    paper_std: 0.029
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Integrated Gradients
    model_key: integrated gradients
    model_plain: Integrated Gradients
    metric_values:
    - null
    - 0.086
    - 0.473
    metric_stds:
    - null
    - 0.046
    - 0.087
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.086
    sort_std: 0.046
    true_value: 0.086
    true_std: 0.046
    paper_value: 0.086
    paper_std: 0.046
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    metric_values:
    - null
    - 0.094
    - 0.49
    metric_stds:
    - null
    - 0.052
    - 0.046
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.094
    sort_std: 0.052
    true_value: 0.094
    true_std: 0.052
    paper_value: 0.094
    paper_std: 0.052
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 3
  - model: Random Node Features
    model_key: random node features
    model_plain: Random Node Features
    metric_values:
    - null
    - 0.105
    - 0.492
    metric_stds:
    - null
    - 0.056
    - 0.046
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.105
    sort_std: 0.056
    true_value: 0.105
    true_std: 0.056
    paper_value: 0.105
    paper_std: 0.056
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 4
  - model: PGMExplainer
    model_key: pgmexplainer
    model_plain: PGMExplainer
    metric_values:
    - null
    - 0.154
    - 0.385
    metric_stds:
    - null
    - 0.083
    - 0.118
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.154
    sort_std: 0.083
    true_value: 0.154
    true_std: 0.083
    paper_value: 0.154
    paper_std: 0.083
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: VanillaGrad
    model_key: vanillagrad
    model_plain: VanillaGrad
    metric_values:
    - null
    - 0.295
    - 0.363
    metric_stds:
    - null
    - 0.078
    - 0.129
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.295
    sort_std: 0.078
    true_value: 0.295
    true_std: 0.078
    paper_value: 0.295
    paper_std: 0.078
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  metrics:
  - Accuracy
  - Unfaithfulness
  - Instability
  primary_metric: Accuracy
  rank_metric: Unfaithfulness
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Unfaithfulness
  - Instability
  metric: Unfaithfulness
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: PubMed
  is_multi_metric: true
  rows:
  - model: GraphLIME
    model_key: graphlime
    model_plain: GraphLIME
    metric_values:
    - null
    - 0.001
    - 0.44
    metric_stds:
    - null
    - 0.001
    - 0.023
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.001
    sort_std: 0.001
    true_value: 0.001
    true_std: 0.001
    paper_value: 0.001
    paper_std: 0.001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Random Node Features
    model_key: random node features
    model_plain: Random Node Features
    metric_values:
    - null
    - 0.002
    - 0.18
    metric_stds:
    - null
    - 0.0
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Random Edges
    model_key: random edges
    model_plain: Random Edges
    metric_values:
    - null
    - 0.002
    - 0.195
    metric_stds:
    - null
    - 0.0
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 3
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    metric_values:
    - null
    - 0.002
    - 0.192
    metric_stds:
    - null
    - 0.0
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 4
  - model: VanillaGrad
    model_key: vanillagrad
    model_plain: VanillaGrad
    metric_values:
    - null
    - 0.003
    - 0.139
    metric_stds:
    - null
    - 0.0
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.003
    sort_std: 0.0
    true_value: 0.003
    true_std: 0.0
    paper_value: 0.003
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Integrated Gradients
    model_key: integrated gradients
    model_plain: Integrated Gradients
    metric_values:
    - null
    - 0.004
    - 0.855
    metric_stds:
    - null
    - 0.0
    - 0.003
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.004
    sort_std: 0.0
    true_value: 0.004
    true_std: 0.0
    paper_value: 0.004
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: GraphMask
    model_key: graphmask
    model_plain: GraphMask
    metric_values:
    - null
    - 0.01
    - 0.742
    metric_stds:
    - null
    - 0.002
    - 0.018
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.01
    sort_std: 0.002
    true_value: 0.01
    true_std: 0.002
    paper_value: 0.01
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: PGMExplainer
    model_key: pgmexplainer
    model_plain: PGMExplainer
    metric_values:
    - null
    - 0.045
    - 0.142
    metric_stds:
    - null
    - 0.003
    - 0.008
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.045
    sort_std: 0.003
    true_value: 0.045
    true_std: 0.003
    paper_value: 0.045
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: PGExplainer
    model_key: pgexplainer
    model_plain: PGExplainer
    metric_values:
    - null
    - 0.094
    - 0.367
    metric_stds:
    - null
    - 0.004
    - 0.006
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.094
    sort_std: 0.004
    true_value: 0.094
    true_std: 0.004
    paper_value: 0.094
    paper_std: 0.004
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 9
  metrics:
  - Accuracy
  - Unfaithfulness
  - Instability
  primary_metric: Accuracy
  rank_metric: Unfaithfulness
  higher_is_better: false
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Unfaithfulness
  - Instability
  metric: Unfaithfulness
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id003
  dataset: ogbn-arxiv
  is_multi_metric: true
  rows:
  - model: GraphLIME
    model_key: graphlime
    model_plain: GraphLIME
    metric_values:
    - null
    - 0.26
    - 0.374
    metric_stds:
    - null
    - 0.003
    - 0.004
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.26
    sort_std: 0.003
    true_value: 0.26
    true_std: 0.003
    paper_value: 0.26
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: PGExplainer
    model_key: pgexplainer
    model_plain: PGExplainer
    metric_values:
    - null
    - 0.338
    - 0.381
    metric_stds:
    - null
    - 0.002
    - 0.001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.338
    sort_std: 0.002
    true_value: 0.338
    true_std: 0.002
    paper_value: 0.338
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: PGMExplainer
    model_key: pgmexplainer
    model_plain: PGMExplainer
    metric_values:
    - null
    - 0.413
    - 0.27
    metric_stds:
    - null
    - 0.002
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.413
    sort_std: 0.002
    true_value: 0.413
    true_std: 0.002
    paper_value: 0.413
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    metric_values:
    - null
    - 0.43
    - 0.376
    metric_stds:
    - null
    - 0.002
    - 0.001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.43
    sort_std: 0.002
    true_value: 0.43
    true_std: 0.002
    paper_value: 0.43
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Random Edges
    model_key: random edges
    model_plain: Random Edges
    metric_values:
    - null
    - 0.431
    - 0.378
    metric_stds:
    - null
    - 0.002
    - 0.001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.431
    sort_std: 0.002
    true_value: 0.431
    true_std: 0.002
    paper_value: 0.431
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: VanillaGrad
    model_key: vanillagrad
    model_plain: VanillaGrad
    metric_values:
    - null
    - 0.528
    - 0.359
    metric_stds:
    - null
    - 0.002
    - 0.001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.528
    sort_std: 0.002
    true_value: 0.528
    true_std: 0.002
    paper_value: 0.528
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Integrated Gradients
    model_key: integrated gradients
    model_plain: Integrated Gradients
    metric_values:
    - null
    - 0.528
    - 0.372
    metric_stds:
    - null
    - 0.002
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.528
    sort_std: 0.002
    true_value: 0.528
    true_std: 0.002
    paper_value: 0.528
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Random Node Features
    model_key: random node features
    model_plain: Random Node Features
    metric_values:
    - null
    - 0.529
    - 0.375
    metric_stds:
    - null
    - 0.002
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.529
    sort_std: 0.002
    true_value: 0.529
    true_std: 0.002
    paper_value: 0.529
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: GraphMask
    model_key: graphmask
    model_plain: GraphMask
    metric_values:
    - null
    - 0.586
    - 0.125
    metric_stds:
    - null
    - 0.001
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.586
    sort_std: 0.001
    true_value: 0.586
    true_std: 0.001
    paper_value: 0.586
    paper_std: 0.001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 9
  metrics:
  - Accuracy
  - Unfaithfulness
  - Instability
  primary_metric: Accuracy
  rank_metric: Unfaithfulness
  higher_is_better: false
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Unfaithfulness
  - Instability
  metric: Unfaithfulness
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id004
  dataset: ogbn-mag
  is_multi_metric: true
  rows:
  - model: GraphLIME
    model_key: graphlime
    model_plain: GraphLIME
    metric_values:
    - null
    - 0.001
    - 0.354
    metric_stds:
    - null
    - 0.0
    - 0.023
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.001
    sort_std: 0.0
    true_value: 0.001
    true_std: 0.0
    paper_value: 0.001
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Random Node Features
    model_key: random node features
    model_plain: Random Node Features
    metric_values:
    - null
    - 0.002
    - 0.373
    metric_stds:
    - null
    - 0.0
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Random Edges
    model_key: random edges
    model_plain: Random Edges
    metric_values:
    - null
    - 0.002
    - 0.376
    metric_stds:
    - null
    - 0.0
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: VanillaGrad
    model_key: vanillagrad
    model_plain: VanillaGrad
    metric_values:
    - null
    - 0.002
    - 0.312
    metric_stds:
    - null
    - 0.0
    - 0.005
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: Integrated Gradients
    model_key: integrated gradients
    model_plain: Integrated Gradients
    metric_values:
    - null
    - 0.002
    - 0.368
    metric_stds:
    - null
    - 0.0
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: PGMExplainer
    model_key: pgmexplainer
    model_plain: PGMExplainer
    metric_values:
    - null
    - 0.002
    - 0.222
    metric_stds:
    - null
    - 0.0
    - 0.006
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: GraphMask
    model_key: graphmask
    model_plain: GraphMask
    metric_values:
    - null
    - 0.002
    - 0.323
    metric_stds:
    - null
    - 0.0
    - 0.003
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    metric_values:
    - null
    - 0.002
    - 0.375
    metric_stds:
    - null
    - 0.0
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
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
  - model: PGExplainer
    model_key: pgexplainer
    model_plain: PGExplainer
    metric_values:
    - null
    - 0.002
    - 0.375
    metric_stds:
    - null
    - 0.0
    - 0.006
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.002
    sort_std: 0.0
    true_value: 0.002
    true_std: 0.0
    paper_value: 0.002
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2106.09078'
    value_gap_source_title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical
      Analysis of GNN Explanation Methods'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-16'
    value_gap_source_date_label: '2021'
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
    date: Jun 16, 2021
    date_display: Jun 2021
    date_iso: '2021-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 9
  metrics:
  - Accuracy
  - Unfaithfulness
  - Instability
  primary_metric: Accuracy
  rank_metric: Unfaithfulness
  higher_is_better: false
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Unfaithfulness
  - Instability
  metric: Unfaithfulness
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
- benchmark: OGB
  datasets:
  - *id003
  - *id004
- benchmark: TU Dortmund
  datasets:
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: PubMed
      dataset_slug: pubmed
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-arxiv
      dataset_slug: ogbn-arxiv
    - dataset: ogbn-mag
      dataset_slug: ogbn-mag
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
main_figure: /figures/2106.09078/main_figure.jpegoptim.jpg
---

