---
title: Adversarial Attack Framework on Graph Embedding Models with Limited Knowledge
arxiv_id: '2105.12419'
source_url: ''
authors:
- name: Heng Chang
  orcid: null
  s2_author_id: '2140312584'
  s2_url: null
- name: Yu Rong
  orcid: null
  s2_author_id: '48537464'
  s2_url: null
- name: Tingyang Xu
  orcid: null
  s2_author_id: '1754673'
  s2_url: null
- name: Wenbing Huang
  orcid: null
  s2_author_id: '123175679'
  s2_url: null
- name: Honglei Zhang
  orcid: null
  s2_author_id: '2143553263'
  s2_url: null
- name: Peng Cui
  orcid: null
  s2_author_id: '143738684'
  s2_url: null
- name: Xin Wang
  orcid: null
  s2_author_id: '2153687490'
  s2_url: null
- name: Wenwu Zhu
  orcid: null
  s2_author_id: '145583986'
  s2_url: null
- name: Junzhou Huang
  orcid: null
  s2_author_id: '1768190'
  s2_url: null
published_date: May 26, 2021
published_date_iso: '2021-05-26'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'With the success of the graph embedding model in both academic and industrial
  areas, the robustness of graph embeddings against adversarial attacks inevitably
  becomes a crucial problem in graph learning. Existing works usually perform the
  attack in a white-box fashion: they need to access the predictions/labels to construct
  their adversarial losses. However, the inaccessibility of predictions/labels makes
  the white-box attack impractical for a real graph learning system. This paper promotes
  current frameworks in a more general and flexible sense -- we consider the ability
  of various types of graph embedding models to remain resilient against black-box
  driven attacks. We investigate the theoretical connection between graph signal processing
  and graph embedding models, and formulate the graph embedding model as a general
  graph signal process with a corresponding graph filter. Therefore, we design a generalized
  adversarial attack framework: GF-Attack. Without accessing any labels and model
  predictions, GF-Attack can perform the attack directly on the graph filter in a
  black-box fashion. We further prove that GF-Attack can perform an effective attack
  without assumption on the number of layers/window-size of graph embedding models.
  To validate the generalization of GF-Attack, we construct GF-Attack on five popular
  graph embedding models. Extensive experiments validate the effectiveness of GF-Attack
  on several benchmark datasets.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- unattacked
- GF-Attack
mrr: 1.0
adjusted_mrr: 0.6667
mrr_dataset_count: 2
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: CiteSeer
  rows:
  - model: GF-Attack
    model_key: gf-attack
    model_plain: GF-Attack
    value: -0.0847
    std: null
    paper_value: -0.0847
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) using single edge perturbation
      under RBA setting. Metric is change in accuracy (percentage).
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.0847
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.0847
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
  - model: A_class
    model_key: a_class
    model_plain: A_class
    value: -0.0542
    std: null
    paper_value: -0.0542
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) using single edge perturbation
      under RBA setting. Metric is change in accuracy (percentage).
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.0542
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.0542
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
  - model: Degree
    model_key: degree
    model_plain: Degree
    value: -0.0417
    std: null
    paper_value: -0.0417
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) using single edge perturbation
      under RBA setting. Metric is change in accuracy (percentage).
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.0417
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.0417
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
  - model: RL-S2V
    model_key: rl-s2v
    model_plain: RL-S2V
    value: -0.0405
    std: null
    paper_value: -0.0405
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) using single edge perturbation
      under RBA setting. Metric is change in accuracy (percentage).
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.0405
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.0405
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
  - model: Random
    model_key: random
    model_plain: Random
    value: -0.0173
    std: null
    paper_value: -0.0173
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) using single edge perturbation
      under RBA and evasion settings. Metric is change in accuracy (percentage).
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.0173
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.0173
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
  rank_metric: Accuracy
  higher_is_better: false
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: Cora
  rows:
  - model: GF-Attack
    model_key: gf-attack
    model_plain: GF-Attack
    value: -0.0556
    std: null
    paper_value: -0.0556
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Single edge perturbation under RBA setting; reported as change
      in accuracy (percentage) relative to unattacked graph.
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: -0.0531
    at_pub_std: null
    at_pub_source_arxiv: '1908.01297'
    at_pub_source_title: A Restricted Black-box Adversarial Framework Towards Attacking
      Graph Embedding Models
    at_pub_source_date_iso: '2019-08-04'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.0024999999999999953
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.0556
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.0556
    sort_std: null
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: A Restricted Black-box Adversarial Framework Towards
      Attacking Graph Embedding Models
    comparison_source_arxiv: '1908.01297'
    is_best: true
    is_std_outlier: false
  - model: RL-S2V
    model_key: rl-s2v
    model_plain: RL-S2V
    value: -0.041
    std: null
    paper_value: -0.041
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Single edge perturbation under RBA setting; reported as change
      in accuracy (percentage) relative to unattacked graph.
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: -0.052
    at_pub_std: null
    at_pub_source_arxiv: '1908.01297'
    at_pub_source_title: A Restricted Black-box Adversarial Framework Towards Attacking
      Graph Embedding Models
    at_pub_source_date_iso: '2019-08-04'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2019-08-04'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: 0.010999999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: -0.052
    true_std: null
    value_gap_source_arxiv: '1908.01297'
    value_gap_source_title: A Restricted Black-box Adversarial Framework Towards Attacking
      Graph Embedding Models
    value_gap_source_is_current_paper: false
    value_gap: 0.010999999999999996
    has_value_note: false
    value_note: ''
    sort_value: -0.052
    sort_std: null
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Restricted Black-box Adversarial Framework Towards
      Attacking Graph Embedding Models
    comparison_source_arxiv: '1908.01297'
    is_best: false
    is_std_outlier: false
  - model: A_class
    model_key: a_class
    model_plain: A_class
    value: -0.0389
    std: null
    paper_value: -0.0389
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Single edge perturbation under RBA setting; reported as change
      in accuracy (percentage) relative to unattacked graph.
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: -0.0296
    at_pub_std: null
    at_pub_source_arxiv: '1908.01297'
    at_pub_source_title: A Restricted Black-box Adversarial Framework Towards Attacking
      Graph Embedding Models
    at_pub_source_date_iso: '2019-08-04'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.009299999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.0389
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.0389
    sort_std: null
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: A Restricted Black-box Adversarial Framework Towards
      Attacking Graph Embedding Models
    comparison_source_arxiv: '1908.01297'
    is_best: false
    is_std_outlier: false
  - model: Degree
    model_key: degree
    model_plain: Degree
    value: -0.035
    std: null
    paper_value: -0.035
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Single edge perturbation under RBA setting; reported as change
      in accuracy (percentage) relative to unattacked graph.
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: -0.0221
    at_pub_std: null
    at_pub_source_arxiv: '1908.01297'
    at_pub_source_title: A Restricted Black-box Adversarial Framework Towards Attacking
      Graph Embedding Models
    at_pub_source_date_iso: '2019-08-04'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.012900000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.035
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.035
    sort_std: null
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: A Restricted Black-box Adversarial Framework Towards
      Attacking Graph Embedding Models
    comparison_source_arxiv: '1908.01297'
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: -0.0181
    std: null
    paper_value: -0.0181
    paper_std: null
    metric: Accuracy
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Single edge perturbation under RBA setting; reported as change
      in accuracy (percentage) relative to unattacked graph.
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: -0.0122
    at_pub_std: null
    at_pub_source_arxiv: '1908.01297'
    at_pub_source_title: A Restricted Black-box Adversarial Framework Towards Attacking
      Graph Embedding Models
    at_pub_source_date_iso: '2019-08-04'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.005900000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.0181
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.0181
    sort_std: null
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: A Restricted Black-box Adversarial Framework Towards
      Attacking Graph Embedding Models
    comparison_source_arxiv: '1908.01297'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: false
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: PubMed
  rows:
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: sagn
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.9517
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
    arxiv_id: '2605.24867'
    title: 'Clustering as Reasoning: A $k$-Means Interpretation of Chain-of-Thought
      Graph Learning'
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    venue: Accepted by ICML 2026
    codebase_url: https://github.com/Uncnbb/KCoT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9517
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: mixhop (lo)
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: graphsage (lo)
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.9511
    std: 0.0036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9511
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: unattacked
    model_key: unattacked
    model_plain: unattacked
    value: 0.804
    std: null
    paper_value: 0.804
    paper_std: null
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification
      accuracy.
    date: May 26, 2021
    date_display: May 2021
    date_iso: '2021-05-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.804
    at_pub_std: null
    at_pub_source_arxiv: '1908.01297'
    at_pub_source_title: A Restricted Black-box Adversarial Framework Towards Attacking
      Graph Embedding Models
    at_pub_source_date_iso: '2019-08-04'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2021-05-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.804
    true_std: null
    value_gap_source_arxiv: '2105.12419'
    value_gap_source_title: Adversarial Attack Framework on Graph Embedding Models
      with Limited Knowledge
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.804
    sort_std: null
    global_rank: 363
    paper_rank: 363
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: PubMed
      dataset_slug: pubmed
---

