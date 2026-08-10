---
title: Learning Graph Augmentations to Learn Graph Representations
arxiv_id: '2201.09830'
source_url: ''
authors:
- name: Kaveh Hassani
  orcid: null
  s2_author_id: '2443055'
  s2_url: null
- name: Amir Hosein Khas Ahmadi
  orcid: null
  s2_author_id: '1516916058'
  s2_url: null
published_date: Jan 24, 2022
published_date_iso: '2022-01-24'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Devising augmentations for graph contrastive learning is challenging due
  to their irregular structure, drastic distribution shifts, and nonequivalent feature
  spaces across datasets. We introduce LG2AR, Learning Graph Augmentations to Learn
  Graph Representations, which is an end-to-end automatic graph augmentation framework
  that helps encoders learn generalizable representations on both node and graph levels.
  LG2AR consists of a probabilistic policy that learns a distribution over augmentations
  and a set of probabilistic augmentation heads that learn distributions over augmentation
  parameters. We show that LG2AR achieves state-of-the-art results on 18 out of 20
  graph-level and node-level benchmarks compared to previous unsupervised models under
  both linear and semi-supervised evaluation protocols. The source code will be released
  here: https://github.com/kavehhassani/lg2ar'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LG2AR + GRU
- LG2AR + DeepSet
- LG2AR + Random
mrr: 0.0093
adjusted_mrr: 0.0093
mrr_dataset_count: 6
benchmark_categories:
- Classic
- TU Dortmund
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 4
  total: 12
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id001
  dataset: Amazon-Photo
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9703
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.926
    std: 0.004
    paper_value: 0.926
    paper_std: 0.004
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9256
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.00040000000000006697
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9669
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.040899999999999936
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 2
    paper_rank: 300
    rank_delta: 298
    rank_delta_abs: 298
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAM-GT
    model_key: dam-gt
    model_plain: DAM-GT
    value: 0.9666
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9643
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 8
    sort_value: 0.9643
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.924
    std: 0.002
    paper_value: 0.924
    paper_std: 0.002
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9242
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9632
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.0391999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 9
    paper_rank: 326
    rank_delta: 317
    rank_delta_abs: 317
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + GRU
    model_key: lg2ar + gru
    model_plain: LG2AR + GRU
    value: 0.941
    std: 0.004
    paper_value: 0.941
    paper_std: 0.004
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.941
    true_std: 0.004
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.941
    sort_std: 0.004
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.932
    std: 0.003
    paper_value: 0.932
    paper_std: 0.003
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9307
    at_pub_std: 0.0038
    at_pub_source_arxiv: '2112.02472'
    at_pub_source_title: Augmentation-Free Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2021-12-05'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2022-06-26'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0013000000000000789
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9337
    true_std: 0.0021
    value_gap_source_arxiv: '2206.12933'
    value_gap_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0016999999999999238
    has_value_note: false
    value_note: ''
    sort_value: 0.9337
    sort_std: 0.0021
    global_rank: 198
    paper_rank: 216
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.922
    std: 0.002
    paper_value: 0.922
    paper_std: 0.002
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9313
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2101.11525'
    at_pub_source_title: Calibrating and Improving Graph Contrastive Learning
    at_pub_source_date_iso: '2021-01-27'
    at_pub_source_date_label: TMLR 2021
    value_gap_source_date_iso: '2024-03-03'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.009299999999999975
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.932
    true_std: 0.006
    value_gap_source_arxiv: '2403.01400'
    value_gap_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    value_gap_source_is_current_paper: false
    value_gap: 0.010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.932
    sort_std: 0.006
    global_rank: 217
    paper_rank: 356
    rank_delta: 139
    rank_delta_abs: 139
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Calibrating and Improving Graph Contrastive Learning
    comparison_source_arxiv: '2101.11525'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.928
    std: 0.005
    paper_value: 0.928
    paper_std: 0.005
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9246
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2112.02472'
    at_pub_source_title: Augmentation-Free Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2021-12-05'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2025-05-25'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.0034000000000000696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9313
    true_std: 0.0017
    value_gap_source_arxiv: '2505.19024'
    value_gap_source_title: Learn Beneficial Noise as Graph Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.0032999999999999696
    has_value_note: false
    value_note: ''
    sort_value: 0.9313
    sort_std: 0.0017
    global_rank: 229
    paper_rank: 265
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.917
    std: 0.001
    paper_value: 0.917
    paper_std: 0.001
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9174
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-03-03'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.931
    true_std: 0.004
    value_gap_source_arxiv: '2403.01400'
    value_gap_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    value_gap_source_is_current_paper: false
    value_gap: 0.014000000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.931
    sort_std: 0.004
    global_rank: 232
    paper_rank: 396
    rank_delta: 164
    rank_delta_abs: 164
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.916
    std: 0.002
    paper_value: 0.916
    paper_std: 0.002
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9161
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9309
    true_std: 0.0008
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.014899999999999913
    has_value_note: false
    value_note: ''
    sort_value: 0.9309
    sort_std: 0.0008
    global_rank: 239
    paper_rank: 400
    rank_delta: 161
    rank_delta_abs: 161
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + DeepSet
    model_key: lg2ar + deepset
    model_plain: LG2AR + DeepSet
    value: 0.926
    std: 0.005
    paper_value: 0.926
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.926
    true_std: 0.005
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.926
    sort_std: 0.005
    global_rank: 301
    paper_rank: 301
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + Random
    model_key: lg2ar + random
    model_plain: LG2AR + Random
    value: 0.924
    std: 0.006
    paper_value: 0.924
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.924
    true_std: 0.006
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.924
    sort_std: 0.006
    global_rank: 332
    paper_rank: 332
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.922
    std: 0.001
    paper_value: 0.922
    paper_std: 0.001
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9224
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9224
    true_std: null
    value_gap_source_arxiv: '2110.15742'
    value_gap_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.9224
    sort_std: null
    global_rank: 349
    paper_rank: 356
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.909
    std: 0.005
    paper_value: 0.909
    paper_std: 0.005
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-25'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9211
    true_std: 0.0032
    value_gap_source_arxiv: '2305.15747'
    value_gap_source_title: Union Subgraph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0121
    has_value_note: false
    value_note: ''
    sort_value: 0.9211
    sort_std: 0.0032
    global_rank: 360
    paper_rank: 440
    rank_delta: 80
    rank_delta_abs: 80
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.916
    std: 0.001
    paper_value: 0.916
    paper_std: 0.001
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9168
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0007999999999999119
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9185
    true_std: 0.0006
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0024999999999999467
    has_value_note: false
    value_note: ''
    sort_value: 0.9185
    sort_std: 0.0006
    global_rank: 385
    paper_rank: 400
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9128
    std: 0.0063
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_display: Jun 2023
    date_iso: '2023-06-04'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: https://github.com/GISec-Team/NCGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 426
    sort_value: 0.9128
    sort_std: 0.0063
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.907
    std: 0.002
    paper_value: 0.907
    paper_std: 0.002
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9068
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2025-12-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9081
    true_std: 0.0015
    value_gap_source_arxiv: '2512.24062'
    value_gap_source_title: Energy-Balanced Hyperspherical Graph Representation Learning
      via Structural Binding and Entropic Dispersion
    value_gap_source_is_current_paper: false
    value_gap: 0.0010999999999999899
    has_value_note: false
    value_note: ''
    sort_value: 0.9081
    sort_std: 0.0015
    global_rank: 447
    paper_rank: 455
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk + feat.
    model_key: deepwalk + feat.
    model_plain: DeepWalk + feat.
    value: 0.901
    std: 0.001
    paper_value: 0.901
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.901
    true_std: 0.001
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.901
    sort_std: 0.001
    global_rank: 486
    paper_rank: 486
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.894
    std: 0.001
    paper_value: 0.894
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9005
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-07-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.00649999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9005
    true_std: 0.0008
    value_gap_source_arxiv: '2307.01053'
    value_gap_source_title: 'ENGAGE: Explanation Guided Data Augmentation for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.00649999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9005
    sort_std: 0.0008
    global_rank: 487
    paper_rank: 509
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.897
    std: 0.001
    paper_value: 0.897
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8967
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-09-12'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.897
    true_std: 0.001
    value_gap_source_arxiv: '2409.08010'
    value_gap_source_title: Multiplex Graph Contrastive Learning with Soft Negatives
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.897
    sort_std: 0.001
    global_rank: 501
    paper_rank: 501
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Raw features
    model_key: raw features
    model_plain: Raw features
    value: 0.785
    std: 0.0
    paper_value: 0.785
    paper_std: 0.0
    metric: Accuracy
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7853
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7999
    true_std: 0.009
    value_gap_source_arxiv: '2506.06212'
    value_gap_source_title: Model-Driven Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.014900000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.7999
    sort_std: 0.009
    global_rank: 584
    paper_rank: 593
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Adaptive Augmentation
    comparison_source_arxiv: '2010.14945'
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
- &id006
  dataset: COLLAB
  rows:
  - model: WL-MLP
    model_key: wl-mlp
    model_plain: WL-MLP
    value: 0.9792
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
    sort_value: 0.9792
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.964
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.964
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CoCN
    model_key: cocn
    model_plain: CoCN
    value: 0.8722
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.18480'
    title: Scalable Graph Compressed Convolutions
    date: Jul 26, 2024
    date_display: Jul 2024
    date_iso: '2024-07-26'
    venue: arXiv.org
    codebase_url: https://github.com/sunjss/CoCN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: use the one-hot encoding of node degrees as node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.8722
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.826
    std: 0.022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.11714'
    title: Scalable Expressiveness through Preprocessed Graph Perturbations
    date: Jun 17, 2024
    date_display: Jun 2024
    date_iso: '2024-06-17'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/Danial-sb/SE2P
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 23
    sort_value: 0.826
    sort_std: 0.022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.707
    std: 0.011
    paper_value: 0.707
    paper_std: 0.011
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
    protocol_note: Linear evaluation protocol using a linear SVM on learned embeddings.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.794
    at_pub_std: null
    at_pub_source_arxiv: '2103.00959'
    at_pub_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    at_pub_source_date_iso: '2021-03-01'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2021-03-01'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.08700000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.794
    true_std: null
    value_gap_source_arxiv: '2103.00959'
    value_gap_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.08700000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.794
    sort_std: null
    global_rank: 151
    paper_rank: 319
    rank_delta: 168
    rank_delta_abs: 168
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    comparison_source_arxiv: '2103.00959'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.792
    std: 0.024
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 157
    sort_value: 0.792
    sort_std: 0.024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + GRU
    model_key: lg2ar + gru
    model_plain: LG2AR + GRU
    value: 0.778
    std: 0.002
    paper_value: 0.778
    paper_std: 0.002
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using a linear SVM on learned embeddings.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.778
    true_std: 0.002
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.002
    global_rank: 194
    paper_rank: 194
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + DeepSet
    model_key: lg2ar + deepset
    model_plain: LG2AR + DeepSet
    value: 0.778
    std: 0.002
    paper_value: 0.778
    paper_std: 0.002
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using a linear SVM on learned embeddings.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.778
    true_std: 0.002
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.002
    global_rank: 195
    paper_rank: 195
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + Random
    model_key: lg2ar + random
    model_plain: LG2AR + Random
    value: 0.776
    std: 0.002
    paper_value: 0.776
    paper_std: 0.002
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using a linear SVM on learned embeddings.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.776
    true_std: 0.002
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.776
    sort_std: 0.002
    global_rank: 201
    paper_rank: 201
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
- &id004
  dataset: Coauthor-CS
  rows:
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.969
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: synthetic graph structures added to the training set
    is_global_top: true
    global_rank: 1
    sort_value: 0.969
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GWN-fa
    model_key: gwn-fa
    model_plain: GWN-fa
    value: 0.9667
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9667
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GWN-sym
    model_key: gwn-sym
    model_plain: GWN-sym
    value: 0.9666
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9593
    std: 0.0025
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 6
    sort_value: 0.9593
    sort_std: 0.0025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.93
    std: 0.003
    paper_value: 0.93
    paper_std: 0.003
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.936
    at_pub_std: 0.015
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9514
    true_std: 0.0025
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.021399999999999975
    has_value_note: false
    value_note: ''
    sort_value: 0.9514
    sort_std: 0.0025
    global_rank: 14
    paper_rank: 76
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.923
    std: 0.002
    paper_value: 0.923
    paper_std: 0.002
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.938
    at_pub_std: 0.004
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.014999999999999902
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9437
    true_std: 0.0028
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.02069999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.9437
    sort_std: 0.0028
    global_rank: 23
    paper_rank: 118
    rank_delta: 95
    rank_delta_abs: 95
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unifying Graph Convolutional Neural Networks and Label
      Propagation
    comparison_source_arxiv: '2002.06755'
    is_best: false
    is_std_outlier: false
  - model: LG2AR + GRU
    model_key: lg2ar + gru
    model_plain: LG2AR + GRU
    value: 0.936
    std: 0.003
    paper_value: 0.936
    paper_std: 0.003
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.936
    true_std: 0.003
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.936
    sort_std: 0.003
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.922
    std: 0.006
    paper_value: 0.922
    paper_std: 0.006
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.922
    at_pub_std: 0.006
    at_pub_source_arxiv: '2111.10698'
    at_pub_source_title: Towards Graph Self-Supervised Learning with Contrastive Adjusted
      Zooming
    at_pub_source_date_iso: '2021-11-20'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.935
    true_std: 0.003
    value_gap_source_arxiv: '2412.21151'
    value_gap_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    value_gap_source_is_current_paper: false
    value_gap: 0.013000000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.935
    sort_std: 0.003
    global_rank: 47
    paper_rank: 123
    rank_delta: 76
    rank_delta_abs: 76
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.931
    std: 0.0
    paper_value: 0.931
    paper_std: 0.0
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9332
    true_std: 0.0012
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: false
    value_gap: 0.0021999999999999797
    has_value_note: false
    value_note: ''
    sort_value: 0.9332
    sort_std: 0.0012
    global_rank: 57
    paper_rank: 69
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.933
    std: 0.001
    paper_value: 0.933
    paper_std: 0.001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9331
    true_std: 0.0013
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.9331
    sort_std: 0.0013
    global_rank: 59
    paper_rank: 60
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.911
    std: 0.002
    paper_value: 0.911
    paper_std: 0.002
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.928
    at_pub_std: 0.001
    at_pub_source_arxiv: '2111.10698'
    at_pub_source_title: Towards Graph Self-Supervised Learning with Contrastive Adjusted
      Zooming
    at_pub_source_date_iso: '2021-11-20'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-02-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.017000000000000015
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9301
    true_std: 0.0003
    value_gap_source_arxiv: '2502.20885'
    value_gap_source_title: A Fused Gromov-Wasserstein Approach to Subgraph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.019100000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9301
    sort_std: 0.0003
    global_rank: 75
    paper_rank: 161
    rank_delta: 86
    rank_delta_abs: 86
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Graph Self-Supervised Learning with Contrastive
      Adjusted Zooming
    comparison_source_arxiv: '2111.10698'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.928
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2412.06173'
    title: Revisiting the Necessity of Graph Learning and Common Graph Benchmarks
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    is_global_top: true
    global_rank: 96
    sort_value: 0.928
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + DeepSet
    model_key: lg2ar + deepset
    model_plain: LG2AR + DeepSet
    value: 0.924
    std: 0.003
    paper_value: 0.924
    paper_std: 0.003
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.924
    true_std: 0.003
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.924
    sort_std: 0.003
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + Random
    model_key: lg2ar + random
    model_plain: LG2AR + Random
    value: 0.923
    std: 0.002
    paper_value: 0.923
    paper_std: 0.002
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.923
    true_std: 0.002
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.923
    sort_std: 0.002
    global_rank: 119
    paper_rank: 119
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.921
    std: 0.001
    paper_value: 0.921
    paper_std: 0.001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9211
    at_pub_std: 0.09
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9211
    true_std: 0.0009
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.9211
    sort_std: 0.0009
    global_rank: 127
    paper_rank: 128
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.921
    std: 0.001
    paper_value: 0.921
    paper_std: 0.001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9211
    at_pub_std: 0.12
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9211
    true_std: 0.0012
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.9211
    sort_std: 0.0012
    global_rank: 126
    paper_rank: 128
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.914
    std: 0.002
    paper_value: 0.914
    paper_std: 0.002
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.914
    true_std: 0.002
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.914
    sort_std: 0.002
    global_rank: 150
    paper_rank: 150
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Raw features
    model_key: raw features
    model_plain: Raw features
    value: 0.904
    std: 0.0
    paper_value: 0.904
    paper_std: 0.0
    metric: Accuracy
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
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9037
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.000300000000000078
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.904
    true_std: 0.0
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.0
    global_rank: 172
    paper_rank: 172
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Contrastive Learning with Adaptive Augmentation
    comparison_source_arxiv: '2010.14945'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.9
    std: 0.007
    paper_value: 0.9
    paper_std: 0.007
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9001
    at_pub_std: 0.71
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9005
    true_std: 0.0035
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 0.0004999999999999449
    has_value_note: false
    value_note: ''
    sort_value: 0.9005
    sort_std: 0.0035
    global_rank: 179
    paper_rank: 179
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk + feat.
    model_key: deepwalk + feat.
    model_plain: DeepWalk + feat.
    value: 0.877
    std: 0.0
    paper_value: 0.877
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.877
    true_std: 0.0
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.877
    sort_std: 0.0
    global_rank: 192
    paper_rank: 192
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.851
    std: 0.0
    paper_value: 0.851
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8508
    at_pub_std: 0.03
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.851
    true_std: 0.0
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.851
    sort_std: 0.0
    global_rank: 201
    paper_rank: 201
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.846
    std: 0.002
    paper_value: 0.846
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using 2-layer GCN encoder, mean accuracy
      over 20 runs.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8461
    at_pub_std: 0.22
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8461
    true_std: 0.0022
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.8461
    sort_std: 0.0022
    global_rank: 205
    paper_rank: 205
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: Coauthor-Physics
  rows:
  - model: GrokFormer
    model_key: grokformer
    model_plain: GrokFormer
    value: 0.9831
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9831
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PolyFormer
    model_key: polyformer
    model_plain: PolyFormer
    value: 0.9808
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9808
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.9796
    std: 0.0081
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9796
    sort_std: 0.0081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.955
    std: 0.002
    paper_value: 0.955
    paper_std: 0.002
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.962
    at_pub_std: 0.001
    at_pub_source_arxiv: '2103.14958'
    at_pub_source_title: 'SelfGNN: Self-supervised Graph Neural Networks without explicit
      negative sampling'
    at_pub_source_date_iso: '2021-03-27'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.007000000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9782
    true_std: 0.0028
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.0232
    has_value_note: false
    value_note: ''
    sort_value: 0.9782
    sort_std: 0.0028
    global_rank: 6
    paper_rank: 141
    rank_delta: 135
    rank_delta_abs: 135
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SelfGNN: Self-supervised Graph Neural Networks without
      explicit negative sampling'
    comparison_source_arxiv: '2103.14958'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.957
    std: 0.002
    paper_value: 0.957
    paper_std: 0.002
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.965
    at_pub_std: 0.001
    at_pub_source_arxiv: '2103.14958'
    at_pub_source_title: 'SelfGNN: Self-supervised Graph Neural Networks without explicit
      negative sampling'
    at_pub_source_date_iso: '2021-03-27'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.008000000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9774
    true_std: 0.0035
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.020400000000000085
    has_value_note: false
    value_note: ''
    sort_value: 0.9774
    sort_std: 0.0035
    global_rank: 9
    paper_rank: 109
    rank_delta: 100
    rank_delta_abs: 100
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SelfGNN: Self-supervised Graph Neural Networks without
      explicit negative sampling'
    comparison_source_arxiv: '2103.14958'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9739
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_display: Jun 2023
    date_iso: '2023-06-04'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: https://github.com/GISec-Team/NCGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 18
    sort_value: 0.9739
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9597
    std: 0.0007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 83
    sort_value: 0.9597
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.957
    std: 0.0
    paper_value: 0.957
    paper_std: 0.0
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9573
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-10-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.000300000000000078
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.959
    true_std: 0.002
    value_gap_source_arxiv: '2210.08792'
    value_gap_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.959
    sort_std: 0.002
    global_rank: 88
    paper_rank: 109
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.957
    std: 0.001
    paper_value: 0.957
    paper_std: 0.001
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9556
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-10-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0013999999999999568
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.958
    true_std: 0.004
    value_gap_source_arxiv: '2210.08792'
    value_gap_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.958
    sort_std: 0.004
    global_rank: 94
    paper_rank: 109
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: LG2AR + GRU
    model_key: lg2ar + gru
    model_plain: LG2AR + GRU
    value: 0.957
    std: 0.002
    paper_value: 0.957
    paper_std: 0.002
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.957
    true_std: 0.002
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.957
    sort_std: 0.002
    global_rank: 113
    paper_rank: 113
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + DeepSet
    model_key: lg2ar + deepset
    model_plain: LG2AR + DeepSet
    value: 0.955
    std: 0.001
    paper_value: 0.955
    paper_std: 0.001
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.955
    true_std: 0.001
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.955
    sort_std: 0.001
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.953
    std: 0.0
    paper_value: 0.953
    paper_std: 0.0
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9533
    at_pub_std: 0.0003
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.000300000000000078
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9544
    true_std: 0.0027
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 0.0014000000000000679
    has_value_note: false
    value_note: ''
    sort_value: 0.9544
    sort_std: 0.0027
    global_rank: 150
    paper_rank: 160
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Adaptive Augmentation
    comparison_source_arxiv: '2010.14945'
    is_best: false
    is_std_outlier: false
  - model: LG2AR + Random
    model_key: lg2ar + random
    model_plain: LG2AR + Random
    value: 0.954
    std: 0.001
    paper_value: 0.954
    paper_std: 0.001
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.954
    true_std: 0.001
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.954
    sort_std: 0.001
    global_rank: 152
    paper_rank: 152
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.952
    std: 0.001
    paper_value: 0.952
    paper_std: 0.001
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.953
    true_std: 0.001
    value_gap_source_arxiv: '2403.05064'
    value_gap_source_title: Unsupervised Graph Neural Architecture Search with Disentangled
      Self-supervision
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.953
    sort_std: 0.001
    global_rank: 161
    paper_rank: 168
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.9492
    std: 0.001
    paper_value: 0.9492
    paper_std: 0.001
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9492
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.952
    true_std: 0.001
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.0027999999999999137
    has_value_note: false
    value_note: ''
    sort_value: 0.952
    sort_std: 0.001
    global_rank: 170
    paper_rank: 185
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.918
    std: 0.002
    paper_value: 0.918
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.949
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.030999999999999917
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.949
    true_std: null
    value_gap_source_arxiv: '2110.15742'
    value_gap_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.030999999999999917
    has_value_note: false
    value_note: ''
    sort_value: 0.949
    sort_std: null
    global_rank: 188
    paper_rank: 293
    rank_delta: 105
    rank_delta_abs: 105
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: DeepWalk + feat.
    model_key: deepwalk + feat.
    model_plain: DeepWalk + feat.
    value: 0.949
    std: 0.001
    paper_value: 0.949
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-06'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.949
    true_std: 0.0009
    value_gap_source_arxiv: '2306.04004'
    value_gap_source_title: Randomized Schur Complement Views for Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.949
    sort_std: 0.0009
    global_rank: 186
    paper_rank: 186
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.945
    std: 0.005
    paper_value: 0.945
    paper_std: 0.005
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9451
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.00010000000000010001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9489
    true_std: 0.0009
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.0039000000000000146
    has_value_note: false
    value_note: ''
    sort_value: 0.9489
    sort_std: 0.0009
    global_rank: 191
    paper_rank: 199
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.945
    std: 0.0
    paper_value: 0.945
    paper_std: 0.0
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9452
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-01-31'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: 0.000200000000000089
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9452
    true_std: 0.0
    value_gap_source_arxiv: '2401.17580'
    value_gap_source_title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    value_gap_source_is_current_paper: false
    value_gap: 0.000200000000000089
    has_value_note: false
    value_note: ''
    sort_value: 0.9452
    sort_std: 0.0
    global_rank: 199
    paper_rank: 199
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Adaptive Augmentation
    comparison_source_arxiv: '2010.14945'
    is_best: false
    is_std_outlier: false
  - model: Raw features
    model_key: raw features
    model_plain: Raw features
    value: 0.936
    std: 0.0
    paper_value: 0.936
    paper_std: 0.0
    metric: Accuracy
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9358
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.000200000000000089
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9432
    true_std: 0.0014
    value_gap_source_arxiv: '2506.06212'
    value_gap_source_title: Model-Driven Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.007199999999999984
    has_value_note: false
    value_note: ''
    sort_value: 0.9432
    sort_std: 0.0014
    global_rank: 207
    paper_rank: 232
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Contrastive Learning with Adaptive Augmentation
    comparison_source_arxiv: '2010.14945'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.912
    std: 0.0
    paper_value: 0.912
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Mean accuracy over 20 runs under linear evaluation protocol using
      GCN encoder.
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9119
    at_pub_std: 0.0004
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2022-10-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.912
    true_std: 0.001
    value_gap_source_arxiv: '2210.08792'
    value_gap_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.912
    sort_std: 0.001
    global_rank: 299
    paper_rank: 299
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: MUTAG
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.991
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ID-GNN+BEC
    model_key: id-gnn+bec
    model_plain: ID-GNN+BEC
    value: 0.983
    std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SupCosine
    model_key: supcosine
    model_plain: SupCosine
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.894
    std: 0.056
    paper_value: 0.894
    paper_std: 0.056
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
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.933
    at_pub_std: 0.029
    at_pub_source_arxiv: '2112.00911'
    at_pub_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    at_pub_source_date_iso: '2021-12-02'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-12-02'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.039000000000000035
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.933
    true_std: 0.029
    value_gap_source_arxiv: '2112.00911'
    value_gap_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.039000000000000035
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.029
    global_rank: 43
    paper_rank: 254
    rank_delta: 211
    rank_delta_abs: 211
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.856
    std: 0.058
    paper_value: 0.856
    paper_std: 0.058
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
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.891
    at_pub_std: 0.0581
    at_pub_source_arxiv: '2106.04319'
    at_pub_source_title: Breaking the Limits of Message Passing Graph Neural Networks
    at_pub_source_date_iso: '2021-06-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-03-03'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.03500000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.922
    true_std: 0.044
    value_gap_source_arxiv: '2503.01079'
    value_gap_source_title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery
      Curvature
    value_gap_source_is_current_paper: false
    value_gap: 0.06600000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.922
    sort_std: 0.044
    global_rank: 71
    paper_rank: 465
    rank_delta: 394
    rank_delta_abs: 394
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.807
    std: 0.03
    paper_value: 0.807
    paper_std: 0.03
    metric: Accuracy
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.904
    at_pub_std: 0.057
    at_pub_source_arxiv: '1912.06058'
    at_pub_source_title: Coloring graph neural networks for node disambiguation
    at_pub_source_date_iso: '2019-12-12'
    at_pub_source_date_label: IJCAI 2019
    value_gap_source_date_iso: '2023-05-23'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.09699999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.904
    true_std: 0.057
    value_gap_source_arxiv: '2305.13987'
    value_gap_source_title: On Structural Expressive Power of Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.09699999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.057
    global_rank: 171
    paper_rank: 660
    rank_delta: 489
    rank_delta_abs: 489
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Coloring graph neural networks for node disambiguation
    comparison_source_arxiv: '1912.06058'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.904
    std: 0.078
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.12245'
    title: Asynchronous Neural Networks for Learning in Graphs
    date: May 24, 2022
    date_display: May 2022
    date_iso: '2022-05-24'
    venue: arXiv.org
    codebase_url: https://github.com/beabevi/ESAN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 170
    sort_value: 0.904
    sort_std: 0.078
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.894
    std: 0.061
    paper_value: 0.894
    paper_std: 0.061
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
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.901
    at_pub_std: 0.0584
    at_pub_source_arxiv: '2106.04319'
    at_pub_source_title: Breaking the Limits of Message Passing Graph Neural Networks
    at_pub_source_date_iso: '2021-06-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-08-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.007000000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.901
    true_std: 0.058
    value_gap_source_arxiv: '2308.08235'
    value_gap_source_title: 'The Expressive Power of Graph Neural Networks: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.007000000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.901
    sort_std: 0.058
    global_rank: 196
    paper_rank: 254
    rank_delta: 58
    rank_delta_abs: 58
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + GRU
    model_key: lg2ar + gru
    model_plain: LG2AR + GRU
    value: 0.9
    std: 0.006
    paper_value: 0.9
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9
    true_std: 0.006
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9
    sort_std: 0.006
    global_rank: 208
    paper_rank: 208
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ADGCL
    model_key: adgcl
    model_plain: ADGCL
    value: 0.897
    std: 0.01
    paper_value: 0.897
    paper_std: 0.01
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
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.897
    true_std: 0.01
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.897
    sort_std: 0.01
    global_rank: 231
    paper_rank: 231
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.89
    std: 0.011
    paper_value: 0.89
    paper_std: 0.011
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
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8901
    at_pub_std: 0.0113
    at_pub_source_arxiv: '2106.07594'
    at_pub_source_title: Graph Contrastive Learning Automated
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.893
    true_std: 0.0514
    value_gap_source_arxiv: '2305.19903'
    value_gap_source_title: Improving Expressivity of GNNs with Subgraph-specific
      Factor Embedded Normalization
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.893
    sort_std: 0.0514
    global_rank: 273
    paper_rank: 289
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + DeepSet
    model_key: lg2ar + deepset
    model_plain: LG2AR + DeepSet
    value: 0.889
    std: 0.006
    paper_value: 0.889
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.889
    true_std: 0.006
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.889
    sort_std: 0.006
    global_rank: 300
    paper_rank: 300
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + Random
    model_key: lg2ar + random
    model_plain: LG2AR + Random
    value: 0.886
    std: 0.005
    paper_value: 0.886
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.886
    true_std: 0.005
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.886
    sort_std: 0.005
    global_rank: 324
    paper_rank: 324
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
    value: 0.868
    std: 0.014
    paper_value: 0.868
    paper_std: 0.014
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
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.868
    at_pub_std: 0.0134
    at_pub_source_arxiv: '2106.07594'
    at_pub_source_title: Graph Contrastive Learning Automated
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-05-25'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8829
    true_std: 0.0131
    value_gap_source_arxiv: '2505.19024'
    value_gap_source_title: Learn Beneficial Noise as Graph Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.014900000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.8829
    sort_std: 0.0131
    global_rank: 342
    paper_rank: 422
    rank_delta: 80
    rank_delta_abs: 80
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLG
    model_key: mlg
    model_plain: MLG
    value: 0.879
    std: 0.016
    paper_value: 0.879
    paper_std: 0.016
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8794
    at_pub_std: 0.0161
    at_pub_source_arxiv: '1603.06186'
    at_pub_source_title: The Multiscale Laplacian Graph Kernel
    at_pub_source_date_iso: '2016-03-01'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8794
    true_std: 0.0161
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.8794
    sort_std: 0.0161
    global_rank: 352
    paper_rank: 354
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.877
    std: 0.008
    paper_value: 0.877
    paper_std: 0.008
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
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.877
    at_pub_std: null
    at_pub_source_arxiv: '2103.00111'
    at_pub_source_title: 'Graph Self-Supervised Learning: A Survey'
    at_pub_source_date_iso: '2021-02-27'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.877
    true_std: 0.008
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.877
    sort_std: 0.008
    global_rank: 371
    paper_rank: 371
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.874
    std: 0.027
    paper_value: 0.874
    paper_std: 0.027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8744
    at_pub_std: 0.027
    at_pub_source_arxiv: '1905.11136'
    at_pub_source_title: Provably Powerful Graph Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8744
    true_std: 0.0272
    value_gap_source_arxiv: '2506.06212'
    value_gap_source_title: Model-Driven Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.8744
    sort_std: 0.0272
    global_rank: 385
    paper_rank: 386
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.866
    std: 0.0495
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.04319'
    title: Breaking the Limits of Message Passing Graph Neural Networks
    date: Jun 8, 2021
    date_display: Jun 2021
    date_iso: '2021-06-08'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/balcilar/gnn-matlang
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 430
    sort_value: 0.866
    sort_std: 0.0495
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: graph2vec
    model_key: graph2vec
    model_plain: graph2vec
    value: 0.832
    std: 0.096
    paper_value: 0.832
    paper_std: 0.096
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8368
    at_pub_std: null
    at_pub_source_arxiv: '2103.00959'
    at_pub_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    at_pub_source_date_iso: '2021-03-01'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0048000000000000265
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8644
    true_std: 0.0125
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.032399999999999984
    has_value_note: false
    value_note: ''
    sort_value: 0.8644
    sort_std: 0.0125
    global_rank: 434
    paper_rank: 569
    rank_delta: 135
    rank_delta_abs: 135
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SP
    model_key: sp
    model_plain: SP
    value: 0.852
    std: 0.024
    paper_value: 0.852
    paper_std: 0.024
    metric: Accuracy
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.858
    at_pub_std: 0.002
    at_pub_source_arxiv: '1410.3314'
    at_pub_source_title: Propagation Kernels
    at_pub_source_date_iso: '2014-10-13'
    at_pub_source_date_label: '2014'
    value_gap_source_date_iso: '2014-10-13'
    value_gap_source_date_label: '2014'
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.858
    true_std: 0.002
    value_gap_source_arxiv: '1410.3314'
    value_gap_source_title: Propagation Kernels
    value_gap_source_is_current_paper: false
    value_gap: 0.006000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.858
    sort_std: 0.002
    global_rank: 456
    paper_rank: 479
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Sub2Vec
    model_key: sub2vec
    model_plain: Sub2Vec
    value: 0.611
    std: 0.158
    paper_value: 0.611
    paper_std: 0.158
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.616
    at_pub_std: 0.158
    at_pub_source_arxiv: '2103.13125'
    at_pub_source_title: Learning Graph Representation by Aggregating Subgraphs via
      Mutual Information Maximization
    at_pub_source_date_iso: '2021-03-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8447
    true_std: 0.0037
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.23370000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8447
    sort_std: 0.0037
    global_rank: 514
    paper_rank: 863
    rank_delta: 349
    rank_delta_abs: 349
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: random walk
    model_key: random walk
    model_plain: random walk
    value: 0.837
    std: 0.015
    paper_value: 0.837
    paper_std: 0.015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.837
    at_pub_std: 0.015
    at_pub_source_arxiv: '2006.05582'
    at_pub_source_title: Contrastive Multi-View Representation Learning on Graphs
    at_pub_source_date_iso: '2020-06-01'
    at_pub_source_date_label: ICML 2020
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.837
    true_std: 0.015
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.837
    sort_std: 0.015
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
  - model: GK
    model_key: gk
    model_plain: GK
    value: 0.817
    std: 0.021
    paper_value: 0.817
    paper_std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.835
    at_pub_std: 0.006
    at_pub_source_arxiv: '2101.08170'
    at_pub_source_title: 'SUGAR: Subgraph Neural Network with Reinforcement Pooling
      and Self-Supervised Mutual Information Mechanism'
    at_pub_source_date_iso: '2021-01-20'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2022-03-15'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.018000000000000016
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.835
    true_std: 0.006
    value_gap_source_arxiv: '2203.07691'
    value_gap_source_title: Supervised Contrastive Learning with Structure Inference
      for Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.018000000000000016
    has_value_note: false
    value_note: ''
    sort_value: 0.835
    sort_std: 0.006
    global_rank: 559
    paper_rank: 636
    rank_delta: 77
    rank_delta_abs: 77
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.726
    std: 0.102
    paper_value: 0.726
    paper_std: 0.102
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: linear evaluation protocol
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7263
    at_pub_std: 0.102
    at_pub_source_arxiv: '2106.07594'
    at_pub_source_title: Graph Contrastive Learning Automated
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7263
    true_std: 0.102
    value_gap_source_arxiv: '2506.06212'
    value_gap_source_title: Model-Driven Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.7263
    sort_std: 0.102
    global_rank: 819
    paper_rank: 819
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
- &id003
  dataset: WikiCS
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.772
    std: 0.001
    paper_value: 0.772
    paper_std: 0.001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9302
    true_std: 0.0011
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.1582
    has_value_note: false
    value_note: ''
    sort_value: 0.9302
    sort_std: 0.0011
    global_rank: 1
    paper_rank: 202
    rank_delta: 201
    rank_delta_abs: 201
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RSE + RGCN (70b)
    model_key: rse + rgcn (70b)
    model_plain: RSE + RGCN (70b)
    value: 0.8852
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 2
    sort_value: 0.8852
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LEMP+T
    model_key: lemp+t
    model_plain: LEMP+T
    value: 0.8825
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8825
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8771
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 9
    sort_value: 0.8771
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.777
    std: 0.001
    paper_value: 0.777
    paper_std: 0.001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8533
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07629999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.8533
    sort_std: null
    global_rank: 31
    paper_rank: 186
    rank_delta: 155
    rank_delta_abs: 155
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.759
    std: 0.007
    paper_value: 0.759
    paper_std: 0.007
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8303
    true_std: 0.0021
    value_gap_source_arxiv: '2405.18581'
    value_gap_source_title: 'Unleashing the Potential of Text-attributed Graphs: Automatic
      Relation Decomposition via Large Language Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.07130000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8303
    sort_std: 0.0021
    global_rank: 54
    paper_rank: 220
    rank_delta: 166
    rank_delta_abs: 166
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.801
    std: 0.005
    paper_value: 0.801
    paper_std: 0.005
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8014
    at_pub_std: 0.48
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8014
    true_std: 0.0048
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.8014
    sort_std: 0.0048
    global_rank: 94
    paper_rank: 96
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.8
    std: 0.001
    paper_value: 0.8
    paper_std: 0.001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7998
    at_pub_std: 0.1
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.000200000000000089
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8
    true_std: 0.001
    value_gap_source_arxiv: '2412.21151'
    value_gap_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.001
    global_rank: 100
    paper_rank: 100
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.754
    std: 0.001
    paper_value: 0.754
    paper_std: 0.001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7535
    at_pub_std: 0.14
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2025-07-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.000500000000000056
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7865
    true_std: 0.069
    value_gap_source_arxiv: '2507.19526'
    value_gap_source_title: Quantizing Text-attributed Graphs for Semantic-Structural
      Integration
    value_gap_source_is_current_paper: false
    value_gap: 0.03249999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7865
    sort_std: 0.069
    global_rank: 152
    paper_rank: 228
    rank_delta: 76
    rank_delta_abs: 76
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.784
    std: 0.001
    paper_value: 0.784
    paper_std: 0.001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7835
    at_pub_std: 0.05
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.000500000000000056
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.784
    true_std: 0.001
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.784
    sort_std: 0.001
    global_rank: 163
    paper_rank: 163
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.702
    std: 0.0
    paper_value: 0.702
    paper_std: 0.0
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7015
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0004999999999999449
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7787
    true_std: 0.0053
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.07669999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7787
    sort_std: 0.0053
    global_rank: 181
    paper_rank: 268
    rank_delta: 87
    rank_delta_abs: 87
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.756
    std: 0.002
    paper_value: 0.756
    paper_std: 0.002
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7563
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7787
    true_std: 0.0053
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.022699999999999942
    has_value_note: false
    value_note: ''
    sort_value: 0.7787
    sort_std: 0.0053
    global_rank: 180
    paper_rank: 224
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + GRU
    model_key: lg2ar + gru
    model_plain: LG2AR + GRU
    value: 0.778
    std: 0.005
    paper_value: 0.778
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.778
    true_std: 0.005
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.005
    global_rank: 185
    paper_rank: 185
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.775
    std: 0.0
    paper_value: 0.775
    paper_std: 0.0
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7752
    at_pub_std: 0.08
    at_pub_source_arxiv: '2106.02466'
    at_pub_source_title: 'Graph Barlow Twins: A self-supervised representation learning
      framework for graphs'
    at_pub_source_date_iso: '2021-06-04'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7757
    true_std: 0.0046
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.0006999999999999229
    has_value_note: false
    value_note: ''
    sort_value: 0.7757
    sort_std: 0.0046
    global_rank: 190
    paper_rank: 193
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.744
    std: 0.001
    paper_value: 0.744
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7721
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.028100000000000014
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7721
    true_std: null
    value_gap_source_arxiv: '2110.15742'
    value_gap_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.028100000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.7721
    sort_std: null
    global_rank: 199
    paper_rank: 238
    rank_delta: 39
    rank_delta_abs: 39
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: DeepWalk + feat.
    model_key: deepwalk + feat.
    model_plain: DeepWalk + feat.
    value: 0.772
    std: 0.0
    paper_value: 0.772
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7721
    at_pub_std: 0.03
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-06-04'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7721
    true_std: 0.03
    value_gap_source_arxiv: '2106.02466'
    value_gap_source_title: 'Graph Barlow Twins: A self-supervised representation
      learning framework for graphs'
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.7721
    sort_std: 0.03
    global_rank: 201
    paper_rank: 202
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + DeepSet
    model_key: lg2ar + deepset
    model_plain: LG2AR + DeepSet
    value: 0.762
    std: 0.009
    paper_value: 0.762
    paper_std: 0.009
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.762
    true_std: 0.009
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.762
    sort_std: 0.009
    global_rank: 219
    paper_rank: 219
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LG2AR + Random
    model_key: lg2ar + random
    model_plain: LG2AR + Random
    value: 0.762
    std: 0.007
    paper_value: 0.762
    paper_std: 0.007
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.762
    true_std: 0.007
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.762
    sort_std: 0.007
    global_rank: 220
    paper_rank: 220
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.749
    std: 0.001
    paper_value: 0.749
    paper_std: 0.001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7485
    at_pub_std: 0.08
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.0004999999999999449
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.749
    true_std: 0.001
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.749
    sort_std: 0.001
    global_rank: 234
    paper_rank: 234
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7469
    std: 0.0085
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.11561'
    title: 'View Space: Learning Representation across Arbitrary Graphs'
    date: Dec 12, 2025
    date_display: Dec 2025
    date_iso: '2025-12-12'
    venue: Accepted to ICML 2026
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 237
    sort_value: 0.7469
    sort_std: 0.0085
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Raw features
    model_key: raw features
    model_plain: Raw features
    value: 0.7198
    std: 0.0
    paper_value: 0.7198
    paper_std: 0.0
    metric: Accuracy
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
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7198
    at_pub_std: 0.0
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2022-09-28'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7198
    true_std: 0.0
    value_gap_source_arxiv: '2209.13964'
    value_gap_source_title: Graph Soft-Contrastive Learning via Neighborhood Ranking
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7198
    sort_std: 0.0
    global_rank: 259
    paper_rank: 259
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.718
    std: 0.001
    paper_value: 0.718
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Linear evaluation protocol using GCN encoder
    date: Jan 24, 2022
    date_display: Jan 2022
    date_iso: '2022-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7179
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2112.02472'
    at_pub_source_title: Augmentation-Free Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2021-12-05'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.718
    true_std: 0.001
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.718
    sort_std: 0.001
    global_rank: 261
    paper_rank: 261
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
  - *id004
- benchmark: TU Dortmund
  datasets:
  - *id005
  - *id006
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Coauthor-Physics
      dataset_slug: coauthor-physics
    - dataset: WikiCS
      dataset_slug: wikics
    - dataset: Coauthor-CS
      dataset_slug: coauthor-cs
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: COLLAB
      dataset_slug: collab
main_figure: /figures/2201.09830/main_figure.jpegoptim.jpg
---

