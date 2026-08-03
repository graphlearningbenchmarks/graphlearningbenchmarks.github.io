---
title: 'CPDG: A Contrastive Pre-Training Method for Dynamic Graph Neural Networks'
arxiv_id: '2307.02813'
source_url: ''
authors:
- name: Yuan-Qi Bei
  orcid: null
  s2_author_id: '2155460174'
  s2_url: null
- name: Haonan Xu
  orcid: null
  s2_author_id: '2108836195'
  s2_url: null
- name: Sheng Zhou
  orcid: null
  s2_author_id: '2156158437'
  s2_url: null
- name: Huixuan Chi
  orcid: null
  s2_author_id: '2093916256'
  s2_url: null
- name: Mengdi Zhang
  orcid: null
  s2_author_id: '48985404'
  s2_url: null
- name: Zhao Li
  orcid: null
  s2_author_id: '2156264636'
  s2_url: null
- name: Jiajun Bu
  orcid: null
  s2_author_id: '2064698184'
  s2_url: null
published_date: Jul 6, 2023
published_date_iso: '2023-07-06'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Dynamic graph data mining has gained popularity in recent years due to the
  rich information contained in dynamic graphs and their widespread use in the real
  world. Despite the advances in dynamic graph neural networks (DGNNs), the rich information
  and diverse downstream tasks have posed significant difficulties for the practical
  application of DGNNs in industrial scenarios. To this end, in this paper, we propose
  to address them by pre-training and present the ontrastive re-Training Method for
  ynamic raph Neural Networks (CPDG). CPDG tackles the challenges of pre-training
  for DGNNs, including generalization capability and long-short term modeling capability,
  through a flexible structural-temporal subgraph sampler along with structural-temporal
  contrastive pre-training schemes. Extensive experiments conducted on both large-scale
  research and industrial dynamic graph datasets show that CPDG outperforms existing
  methods in dynamic graph pre-training for various downstream tasks under three transfer
  settings.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- TGN
- CPDG
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
  - model: CPDG
    model_key: pint
    model_plain: CPDG
    value: 0.6731
    std: 0.002
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2209.15059'
    title: Provably expressive temporal graph networks
    date: Sep 29, 2022
    date_display: Sep 2022
    date_iso: '2022-09-29'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6731
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CPDG
    model_key: cpdg
    model_plain: CPDG
    value: 0.6551
    std: 0.0118
    paper_value: 0.6551
    paper_std: 0.0118
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Time transfer split: first 60% for pre-training, rest for fine-tuning
      (including test).'
    date: Jul 6, 2023
    date_display: Jul 2023
    date_iso: '2023-07-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6551
    true_std: 0.0118
    value_gap_source_arxiv: '2307.02813'
    value_gap_source_title: 'CPDG: A Contrastive Pre-Training Method for Dynamic Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6551
    sort_std: 0.0118
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
  - model: DyRep
    model_key: dyrep
    model_plain: DyRep
    value: 0.5614
    std: 0.0281
    paper_value: 0.5614
    paper_std: 0.0281
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Time transfer split: first 60% for pre-training, rest for fine-tuning
      (including test).'
    date: Jul 6, 2023
    date_display: Jul 2023
    date_iso: '2023-07-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6291
    at_pub_std: 0.024
    at_pub_source_arxiv: '2209.15059'
    at_pub_source_title: Provably expressive temporal graph networks
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.06769999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6291
    true_std: 0.024
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: false
    value_gap: 0.06769999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.6291
    sort_std: 0.024
    global_rank: 10
    paper_rank: 14
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Provably expressive temporal graph networks
    comparison_source_arxiv: '2209.15059'
    is_best: false
    is_std_outlier: false
  - model: JODIE
    model_key: jodie
    model_plain: JODIE
    value: 0.5385
    std: 0.0303
    paper_value: 0.5385
    paper_std: 0.0303
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Time transfer split: first 60% for pre-training, rest for fine-tuning
      (including test).'
    date: Jul 6, 2023
    date_display: Jul 2023
    date_iso: '2023-07-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6183
    at_pub_std: 0.027
    at_pub_source_arxiv: '2209.15059'
    at_pub_source_title: Provably expressive temporal graph networks
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.07979999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6183
    true_std: 0.027
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07979999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.6183
    sort_std: 0.027
    global_rank: 11
    paper_rank: 15
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Provably expressive temporal graph networks
    comparison_source_arxiv: '2209.15059'
    is_best: false
    is_std_outlier: false
  - model: TGN
    model_key: tgn
    model_plain: TGN
    value: 0.5552
    std: 0.0106
    paper_value: 0.5552
    paper_std: 0.0106
    metric: AUC
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
    protocol_note: 'Time transfer split: first 60% for pre-training, rest for fine-tuning
      (including test).'
    date: Jul 6, 2023
    date_display: Jul 2023
    date_iso: '2023-07-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5926
    true_std: 0.0041
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: false
    value_gap: 0.03739999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.5926
    sort_std: 0.0041
    global_rank: 13
    paper_rank: 15
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SelfRGNN
    model_key: selfrgnn
    model_plain: SelfRGNN
    value: 0.5363
    std: 0.0051
    paper_value: 0.5363
    paper_std: 0.0051
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Time transfer split: first 60% for pre-training, rest for fine-tuning
      (including test).'
    date: Jul 6, 2023
    date_display: Jul 2023
    date_iso: '2023-07-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5363
    true_std: 0.0051
    value_gap_source_arxiv: '2307.02813'
    value_gap_source_title: 'CPDG: A Contrastive Pre-Training Method for Dynamic Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5363
    sort_std: 0.0051
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DDGCL
    model_key: ddgcl
    model_plain: DDGCL
    value: 0.5205
    std: 0.0207
    paper_value: 0.5205
    paper_std: 0.0207
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Time transfer split: first 60% for pre-training, rest for fine-tuning
      (including test).'
    date: Jul 6, 2023
    date_display: Jul 2023
    date_iso: '2023-07-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5205
    true_std: 0.0207
    value_gap_source_arxiv: '2307.02813'
    value_gap_source_title: 'CPDG: A Contrastive Pre-Training Method for Dynamic Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5205
    sort_std: 0.0207
    global_rank: 19
    paper_rank: 19
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
---

