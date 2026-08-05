---
title: Learning and Evaluating Graph Neural Network Explanations based on Counterfactual
  and Factual Reasoning
arxiv_id: '2202.08816'
source_url: ''
authors:
- name: Juntao Tan
  orcid: null
  s2_author_id: '2110449137'
  s2_url: null
- name: Shijie Geng
  orcid: null
  s2_author_id: '1947101'
  s2_url: null
- name: Zuohui Fu
  orcid: null
  s2_author_id: '2011378'
  s2_url: null
- name: Yingqiang Ge
  orcid: null
  s2_author_id: '152988336'
  s2_url: null
- name: Shuyuan Xu
  orcid: null
  s2_author_id: '2111044480'
  s2_url: null
- name: Yunqi Li
  orcid: null
  s2_author_id: '48515097'
  s2_url: null
- name: Yongfeng Zhang
  orcid: null
  s2_author_id: '1591136873'
  s2_url: null
published_date: Feb 17, 2022
published_date_iso: '2022-02-17'
published_venue: WWW 2022
published_conference: WWW 2022
published_conference_short: WWW
published_conference_slug: www
abstract: Structural data well exists in Web applications, such as social networks
  in social media, citation networks in academic websites, and threads data in online
  forums. Due to the complex topology, it is difficult to process and make use of
  the rich information within such data. Graph Neural Networks (GNNs) have shown great
  advantages on learning representations for structural data. However, the non-transparency
  of the deep learning models makes it non-trivial to explain and interpret the predictions
  made by GNNs. Meanwhile, it is also a big challenge to evaluate the GNN explanations,
  since in many cases, the ground-truth explanations are unavailable. In this paper,
  we take insights of Counterfactual and Factual (CF$^2$) reasoning from causal inference
  theory, to solve both the learning and evaluation problems in explainable GNNs.
  For generating explanations, we propose a model-agnostic framework by formulating
  an optimization problem based on both of the two casual perspectives. This distinguishes
  CF$^2$ from previous explainable GNNs that only consider one of them. Another contribution
  of the work is the evaluation of GNN explanations. For quantitatively evaluating
  the generated explanations without the requirement of ground-truth, we design metrics
  based on Counterfactual and Factual reasoning to evaluate the necessity and sufficiency
  of the explanations. Experiments show that no matter ground-truth explanations are
  available or not, CF$^2$ generates better explanations than previous state-of-the-art
  methods on real-world datasets. Moreover, the statistic analysis justifies the correlation
  between the performance on ground-truth evaluation and our proposed metrics. Source
  code is available at.
codebase_url: https://github.com/chrisjtan/gnn_cff
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CF^2
mrr: 0.0018
adjusted_mrr: 0.0006
mrr_dataset_count: 1
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
  - model: CF^2
    model_key: cf^2
    model_plain: CF^2
    value: 0.987
    std: null
    paper_value: 0.987
    paper_std: null
    metric: F1
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluation using PN/PS-based metrics (F_NS) on test set.
    date: Feb 17, 2022
    date_display: Feb 2022
    date_iso: '2022-02-17'
    published_venue: WWW 2022
    published_conference: WWW 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.987
    true_std: null
    value_gap_source_arxiv: '2202.08816'
    value_gap_source_title: Learning and Evaluating Graph Neural Network Explanations
      based on Counterfactual and Factual Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.987
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
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    value: 0.8267
    std: null
    paper_value: 0.8267
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluation using PN/PS-based metrics (F_NS) on test set.
    date: Feb 17, 2022
    date_display: Feb 2022
    date_iso: '2022-02-17'
    published_venue: WWW 2022
    published_conference: WWW 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8267
    true_std: null
    value_gap_source_arxiv: '2202.08816'
    value_gap_source_title: Learning and Evaluating Graph Neural Network Explanations
      based on Counterfactual and Factual Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8267
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
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.7958
    std: null
    paper_value: 0.7958
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluation using PN/PS-based metrics (F_NS) on test set.
    date: Feb 17, 2022
    date_display: Feb 2022
    date_iso: '2022-02-17'
    published_venue: WWW 2022
    published_conference: WWW 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7958
    true_std: null
    value_gap_source_arxiv: '2202.08816'
    value_gap_source_title: Learning and Evaluating Graph Neural Network Explanations
      based on Counterfactual and Factual Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7958
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
  - model: CF-GNNExplainer
    model_key: cf-gnnexplainer
    model_plain: CF-GNNExplainer
    value: 0.4739
    std: null
    paper_value: 0.4739
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluation of generated explanations against ground-truth motifs
      using test set.
    date: Feb 17, 2022
    date_display: Feb 2022
    date_iso: '2022-02-17'
    published_venue: WWW 2022
    published_conference: WWW 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4739
    true_std: null
    value_gap_source_arxiv: '2202.08816'
    value_gap_source_title: Learning and Evaluating Graph Neural Network Explanations
      based on Counterfactual and Factual Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4739
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
  rank_metric: F1
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: NCI1
  rows:
  - model: WL-MLP
    model_key: wl-mlp
    model_plain: WL-MLP
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8303
    std: 0.0137
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.01794'
    title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based Gnn Explainers
      through In-depth Benchmarking'
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Armagaan/gnn-x-bench
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 81
    sort_value: 0.8303
    sort_std: 0.0137
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.6903
    std: null
    paper_value: 0.6903
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Classification accuracy of the trained base GCN model used for
      explanation.
    date: Feb 17, 2022
    date_display: Feb 2022
    date_iso: '2022-02-17'
    published_venue: WWW 2022
    published_conference: WWW 2022
    at_pub_value: 0.728
    at_pub_std: null
    at_pub_source_arxiv: '2104.06643'
    at_pub_source_title: Generative Causal Explanations for Graph Neural Networks
    at_pub_source_date_iso: '2021-04-14'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2021-04-14'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: 0.037699999999999956
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.728
    true_std: null
    value_gap_source_arxiv: '2104.06643'
    value_gap_source_title: Generative Causal Explanations for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.037699999999999956
    has_value_note: false
    value_note: ''
    sort_value: 0.728
    sort_std: null
    global_rank: 510
    paper_rank: 551
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Generative Causal Explanations for Graph Neural Networks
    comparison_source_arxiv: '2104.06643'
    is_best: false
    is_std_outlier: false
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    value: 0.6903
    std: null
    paper_value: 0.6903
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Classification accuracy of the trained base GCN model used for
      explanation.
    date: Feb 17, 2022
    date_display: Feb 2022
    date_iso: '2022-02-17'
    published_venue: WWW 2022
    published_conference: WWW 2022
    at_pub_value: 0.72
    at_pub_std: null
    at_pub_source_arxiv: '2104.06643'
    at_pub_source_title: Generative Causal Explanations for Graph Neural Networks
    at_pub_source_date_iso: '2021-04-14'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2021-04-14'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: 0.02969999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.72
    true_std: null
    value_gap_source_arxiv: '2104.06643'
    value_gap_source_title: Generative Causal Explanations for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.02969999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.72
    sort_std: null
    global_rank: 517
    paper_rank: 551
    rank_delta: 34
    rank_delta_abs: 34
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Generative Causal Explanations for Graph Neural Networks
    comparison_source_arxiv: '2104.06643'
    is_best: false
    is_std_outlier: false
  - model: CF^2
    model_key: cf^2
    model_plain: CF^2
    value: 0.6903
    std: null
    paper_value: 0.6903
    paper_std: null
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Classification accuracy of the trained base GCN model used for
      explanation.
    date: Feb 17, 2022
    date_display: Feb 2022
    date_iso: '2022-02-17'
    published_venue: WWW 2022
    published_conference: WWW 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6903
    true_std: null
    value_gap_source_arxiv: '2202.08816'
    value_gap_source_title: Learning and Evaluating Graph Neural Network Explanations
      based on Counterfactual and Factual Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6903
    sort_std: null
    global_rank: 553
    paper_rank: 553
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CF-GNNExplainer
    model_key: cf-gnnexplainer
    model_plain: CF-GNNExplainer
    value: 0.6903
    std: null
    paper_value: 0.6903
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Classification accuracy of the trained base GCN model used for
      explanation.
    date: Feb 17, 2022
    date_display: Feb 2022
    date_iso: '2022-02-17'
    published_venue: WWW 2022
    published_conference: WWW 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6903
    true_std: null
    value_gap_source_arxiv: '2202.08816'
    value_gap_source_title: Learning and Evaluating Graph Neural Network Explanations
      based on Counterfactual and Factual Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6903
    sort_std: null
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
single_proposed_model: CF^2
main_figure: /figures/2202.08816/main_figure.jpegoptim.jpg
---

