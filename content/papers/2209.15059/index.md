---
title: Provably expressive temporal graph networks
arxiv_id: '2209.15059'
source_url: ''
authors:
- name: A. Souza
  orcid: null
  s2_author_id: '3383481'
  s2_url: null
- name: Diego Mesquita
  orcid: null
  s2_author_id: '144128644'
  s2_url: null
- name: Samuel Kaski
  orcid: null
  s2_author_id: '1711144'
  s2_url: null
- name: Vikas K. Garg
  orcid: null
  s2_author_id: '2067125028'
  s2_url: null
published_date: Sep 29, 2022
published_date_iso: '2022-09-29'
published_venue: NeurIPS 2022
published_conference: NeurIPS 2022
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: 'Temporal graph networks (TGNs) have gained prominence as models for embedding
  dynamic interactions, but little is known about their theoretical underpinnings.
  We establish fundamental results about the representational power and limits of
  the two main categories of TGNs: those that aggregate temporal walks (WA-TGNs),
  and those that augment local message passing with recurrent memory modules (MP-TGNs).
  Specifically, novel constructions reveal the inadequacy of MP-TGNs and WA-TGNs,
  proving that neither category subsumes the other. We extend the 1-WL (Weisfeiler-Leman)
  test to temporal graphs, and show that the most powerful MP-TGNs should use injective
  updates, as in this case they become as expressive as the temporal WL. Also, we
  show that sufficiently deep MP-TGNs cannot benefit from memory, and MP/WA-TGNs fail
  to compute graph properties such as girth. These theoretical insights lead us to
  PINT --- a novel architecture that leverages injective temporal message passing
  and relative positional features. Importantly, PINT is provably more expressive
  than both MP-TGNs and WA-TGNs. PINT significantly outperforms existing TGNs on several
  real-world benchmarks.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- PINT
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
  dataset: Reddit
  rows:
  - model: CPDG
    model_key: splash
    model_plain: CPDG
    value: 0.7358
    std: 0.0028
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2504.00328'
    title: Simple yet Effective Node Property Prediction on Edge Streams under Distribution
      Shifts
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    venue: IEEE International Conference on Data Engineering
    codebase_url: https://github.com/jhsk777/SPLASH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7358
    sort_std: 0.0028
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CPDG
    model_key: backbone (tgat)
    model_plain: CPDG
    value: 0.6822
    std: 0.0052
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.10673'
    title: 'Less Can Be More: Unsupervised Graph Pruning for Large-scale Dynamic Graphs'
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    venue: arXiv.org
    codebase_url: https://github.com/EdisonLeeeee/STEP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6822
    sort_std: 0.0052
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PINT
    model_key: pint
    model_plain: PINT
    value: 0.6731
    std: 0.002
    paper_value: 0.6731
    paper_std: 0.002
    metric: AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task
    date: Sep 29, 2022
    date_display: Sep 2022
    date_iso: '2022-09-29'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6731
    true_std: 0.002
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6731
    sort_std: 0.002
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
  - model: TGN-Att
    model_key: tgn-att
    model_plain: TGN-Att
    value: 0.6706
    std: 0.009
    paper_value: 0.6706
    paper_std: 0.009
    metric: AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task
    date: Sep 29, 2022
    date_display: Sep 2022
    date_iso: '2022-09-29'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6706
    true_std: 0.009
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6706
    sort_std: 0.009
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
  - model: TGAT
    model_key: tgat
    model_plain: TGAT
    value: 0.6556
    std: 0.007
    paper_value: 0.6556
    paper_std: 0.007
    metric: AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task
    date: Sep 29, 2022
    date_display: Sep 2022
    date_iso: '2022-09-29'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6556
    true_std: 0.007
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6556
    sort_std: 0.007
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
  - model: DyRep
    model_key: dyrep
    model_plain: DyRep
    value: 0.6291
    std: 0.024
    paper_value: 0.6291
    paper_std: 0.024
    metric: AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task
    date: Sep 29, 2022
    date_display: Sep 2022
    date_iso: '2022-09-29'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6291
    true_std: 0.024
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6291
    sort_std: 0.024
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
  - model: JODIE
    model_key: jodie
    model_plain: JODIE
    value: 0.6183
    std: 0.027
    paper_value: 0.6183
    paper_std: 0.027
    metric: AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task
    date: Sep 29, 2022
    date_display: Sep 2022
    date_iso: '2022-09-29'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6183
    true_std: 0.027
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6183
    sort_std: 0.027
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
  - model: CTDNE
    model_key: ctdne
    model_plain: CTDNE
    value: 0.5943
    std: 0.006
    paper_value: 0.5943
    paper_std: 0.006
    metric: AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task
    date: Sep 29, 2022
    date_display: Sep 2022
    date_iso: '2022-09-29'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5943
    true_std: 0.006
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5943
    sort_std: 0.006
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
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - AUC
  metric: AUC
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
    - dataset: Reddit
      dataset_slug: reddit
single_proposed_model: PINT
main_figure: /figures/2209.15059/main_figure.jpegoptim.jpg
---

