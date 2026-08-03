---
title: 'Expressivity of Representation Learning on Continuous-Time Dynamic Graphs:
  An Information-Flow Centric Review'
arxiv_id: '2412.03783'
source_url: ''
authors:
- name: Sofiane Ennadir
  orcid: null
  s2_author_id: '2187458074'
  s2_url: null
- name: Gabriela Zarzar Gandler
  orcid: null
  s2_author_id: '1395612327'
  s2_url: null
- name: Filip Cornell
  orcid: null
  s2_author_id: '2333905810'
  s2_url: null
- name: Lele Cao
  orcid: null
  s2_author_id: '2328683627'
  s2_url: null
- name: Oleg Smirnov
  orcid: null
  s2_author_id: '2295510847'
  s2_url: null
- name: Tianze Wang
  orcid: null
  s2_author_id: '2295697958'
  s2_url: null
- name: Levente Z'olyomi
  orcid: null
  s2_author_id: '2333887053'
  s2_url: null
- name: Bjorn Brinne
  orcid: null
  s2_author_id: '2333895460'
  s2_url: null
- name: Sahar Asadi
  orcid: null
  s2_author_id: '2295512139'
  s2_url: null
published_date: Dec 5, 2024
published_date_iso: '2024-12-05'
published_venue: TMLR 2024
published_conference: TMLR 2024
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: Graphs are ubiquitous in real-world applications, ranging from social networks
  to biological systems, and have inspired the development of Graph Neural Networks
  (GNNs) for learning expressive representations. While most research has centered
  on static graphs, many real-world scenarios involve dynamic, temporally evolving
  graphs, motivating the need for Continuous-Time Dynamic Graph (CTDG) models. This
  paper provides a comprehensive review of Graph Representation Learning (GRL) on
  CTDGs with a focus on Self-Supervised Representation Learning (SSRL). We introduce
  a novel theoretical framework that analyzes the expressivity of CTDG models through
  an Information-Flow (IF) lens, quantifying their ability to propagate and encode
  temporal and structural information. Leveraging this framework, we categorize existing
  CTDG methods based on their suitability for different graph types and application
  scenarios. Within the same scope, we examine the design of SSRL methods tailored
  to CTDGs, such as predictive and contrastive approaches, highlighting their potential
  to mitigate the reliance on labeled data. Empirical evaluations on synthetic and
  real-world datasets validate our theoretical insights, demonstrating the strengths
  and limitations of various methods across long-range, bi-partite and community-based
  graphs. This work offers both a theoretical foundation and practical guidance for
  selecting and developing CTDG models, advancing the understanding of GRL in dynamic
  settings.
codebase_url: https://github.com/king/ctdg-info-flow
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Information-Flow (IF) framework
mrr: 0.1111
adjusted_mrr: 0.037
mrr_dataset_count: 1
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id001
  dataset: ogbl-wikikg2
  rows:
  - model: Information-Flow (IF) framework
    model_key: stargraph + triplere'
    model_plain: Information-Flow (IF) framework
    value: 0.729
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    venue: Under review in ICLR 2023 (https://openreview.net/forum?id=mTOB_VK_BWk)
    codebase_url: https://github.com/hzli-ucas/StarGraph
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.729
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Information-Flow (IF) framework
    model_key: trans(large) + nodepiece
    model_plain: Information-Flow (IF) framework
    value: 0.6939
    std: 0.0011
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 38.430804
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    venue: Under review in ICLR 2023 (https://openreview.net/forum?id=mTOB_VK_BWk)
    codebase_url: https://github.com/hzli-ucas/StarGraph
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6939
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Information-Flow (IF) framework
    model_key: trans + nodepiece
    model_plain: Information-Flow (IF) framework
    value: 0.6882
    std: 0.0019
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.215402
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    venue: Under review in ICLR 2023 (https://openreview.net/forum?id=mTOB_VK_BWk)
    codebase_url: https://github.com/hzli-ucas/StarGraph
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6882
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Information-Flow (IF) framework
    model_key: information-flow (if) framework
    model_plain: Information-Flow (IF) framework
    value: 0.611
    std: 0.011
    paper_value: 0.611
    paper_std: 0.011
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbl-wikikg2 (score=76)'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test split for TGBL-Wiki as per TGB benchmark standards
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-05'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.611
    true_std: 0.011
    value_gap_source_arxiv: '2412.03783'
    value_gap_source_title: 'Expressivity of Representation Learning on Continuous-Time
      Dynamic Graphs: An Information-Flow Centric Review'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.611
    sort_std: 0.011
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
  - model: TGN
    model_key: tgn
    model_plain: TGN
    value: 0.577
    std: 0.015
    paper_value: 0.577
    paper_std: 0.015
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbl-wikikg2 (score=76)'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test split for TGBL-Wiki as per TGB benchmark standards
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-05'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.577
    true_std: 0.015
    value_gap_source_arxiv: '2412.03783'
    value_gap_source_title: 'Expressivity of Representation Learning on Continuous-Time
      Dynamic Graphs: An Information-Flow Centric Review'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.577
    sort_std: 0.015
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
  - model: TGAT
    model_key: tgat
    model_plain: TGAT
    value: 0.282
    std: 0.022
    paper_value: 0.282
    paper_std: 0.022
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbl-wikikg2 (score=76)'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test split for TGBL-Wiki as per TGB benchmark standards
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-05'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.282
    true_std: 0.022
    value_gap_source_arxiv: '2412.03783'
    value_gap_source_title: 'Expressivity of Representation Learning on Continuous-Time
      Dynamic Graphs: An Information-Flow Centric Review'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.282
    sort_std: 0.022
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DyRep
    model_key: dyrep
    model_plain: DyRep
    value: 0.263
    std: 0.005
    paper_value: 0.263
    paper_std: 0.005
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbl-wikikg2 (score=76)'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test split for TGBL-Wiki as per TGB benchmark standards
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-05'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.263
    true_std: 0.005
    value_gap_source_arxiv: '2412.03783'
    value_gap_source_title: 'Expressivity of Representation Learning on Continuous-Time
      Dynamic Graphs: An Information-Flow Centric Review'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.263
    sort_std: 0.005
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
  - model: JODIE
    model_key: jodie
    model_plain: JODIE
    value: 0.261
    std: 0.123
    paper_value: 0.261
    paper_std: 0.123
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbl-wikikg2 (score=76)'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test split for TGBL-Wiki as per TGB benchmark standards
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-05'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.261
    true_std: 0.123
    value_gap_source_arxiv: '2412.03783'
    value_gap_source_title: 'Expressivity of Representation Learning on Continuous-Time
      Dynamic Graphs: An Information-Flow Centric Review'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.261
    sort_std: 0.123
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
    is_std_outlier: true
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbl-wikikg2
      dataset_slug: ogbl-wikikg2
single_proposed_model: Information-Flow (IF) framework
main_figure: /figures/2412.03783/main_figure.jpegoptim.jpg
---

