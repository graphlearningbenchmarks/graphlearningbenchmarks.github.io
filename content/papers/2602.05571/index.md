---
title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures via Adversarial Edge
  Masking'
arxiv_id: '2602.05571'
source_url: ''
authors:
- name: Rishabh Bhattacharya
  orcid: null
  s2_author_id: '2392258928'
  s2_url: null
- name: Naresh Manwani
  orcid: null
  s2_author_id: '3222980'
  s2_url: null
published_date: Feb 5, 2026
published_date_iso: '2026-02-05'
published_venue: TMLR 2026
published_conference: TMLR 2026
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: Structural shifts pose a significant challenge for graph neural networks,
  as graph topology acts as a covariate that can vary across domains. Existing domain
  generalization methods rely on fixed structural augmentations or training on globally
  perturbed graphs, mechanisms that do not pinpoint which specific edges encode domain-invariant
  information. We argue that domain-invariant structural information is not rigidly
  tied to a single topology but resides in the consensus across multiple graph structures
  derived from topology and feature similarity. To capture this, we first propose
  EdgeMask-DG, a novel min-max algorithm where an edge masker learns to find worst-case
  continuous masks subject to a sparsity constraint, compelling a task GNN to perform
  effectively under these adversarial structural perturbations. Building upon this,
  we introduce EdgeMask-DG*, an extension that applies this adversarial masking principle
  to an enriched graph. This enriched graph combines the original topology with feature-derived
  edges, allowing the model to discover invariances even when the original topology
  is noisy or domain-specific. EdgeMask-DG* is the first to systematically combine
  adaptive adversarial topology search with feature-enriched graphs. We provide a
  formal justification for our approach from a robust optimization perspective. We
  demonstrate that EdgeMask-DG* achieves new state-of-the-art performance on diverse
  graph domain generalization benchmarks, including citation networks, social networks,
  and temporal graphs. Notably, on the Cora OOD benchmark, EdgeMask-DG\* lifts the
  worst-case domain accuracy to 78.0\
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Graph-DG
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
    value: 0.9669
    std: 0.0014
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
    global_rank: 2
    sort_value: 0.9669
    sort_std: 0.0014
    comparison_type: global_top
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
  - model: EdgeMask-DG*
    model_key: edgemask-dg
    model_plain: EdgeMask-DG*
    value: 0.948
    std: 0.006
    paper_value: 0.948
    paper_std: 0.006
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.948
    true_std: 0.006
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.948
    sort_std: 0.006
    global_rank: 87
    paper_rank: 87
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRM
    model_key: grm
    model_plain: GRM
    value: 0.927
    std: 0.016
    paper_value: 0.927
    paper_std: 0.016
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
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.927
    true_std: 0.016
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.927
    sort_std: 0.016
    global_rank: 289
    paper_rank: 289
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EERM
    model_key: eerm
    model_plain: EERM
    value: 0.918
    std: 0.009
    paper_value: 0.918
    paper_std: 0.009
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
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: 0.9079
    at_pub_std: 0.0218
    at_pub_source_arxiv: '2408.01697'
    at_pub_source_title: Invariant Graph Learning Meets Information Bottleneck for
      Out-of-Distribution Generalization
    at_pub_source_date_iso: '2024-08-03'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: 0.010099999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.918
    true_std: 0.009
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.918
    sort_std: 0.009
    global_rank: 390
    paper_rank: 390
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LiSA
    model_key: lisa
    model_plain: LiSA
    value: 0.915
    std: 0.015
    paper_value: 0.915
    paper_std: 0.015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.915
    true_std: 0.015
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.915
    sort_std: 0.015
    global_rank: 410
    paper_rank: 410
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
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
  - model: IS-GIB
    model_key: is-gib
    model_plain: IS-GIB
    value: 0.902
    std: 0.009
    paper_value: 0.902
    paper_std: 0.009
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.902
    true_std: 0.009
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.902
    sort_std: 0.009
    global_rank: 483
    paper_rank: 483
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MARIO
    model_key: mario
    model_plain: MARIO
    value: 0.894
    std: 0.014
    paper_value: 0.894
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.894
    true_std: 0.014
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: 0.014
    global_rank: 510
    paper_rank: 510
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ERM
    model_key: erm
    model_plain: ERM
    value: 0.886
    std: 0.013
    paper_value: 0.886
    paper_std: 0.013
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
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: 0.8806
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2408.01697'
    at_pub_source_title: Invariant Graph Learning Meets Information Bottleneck for
      Out-of-Distribution Generalization
    at_pub_source_date_iso: '2024-08-03'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: 0.00539999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.886
    true_std: 0.013
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.886
    sort_std: 0.013
    global_rank: 531
    paper_rank: 531
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MMD
    model_key: mmd
    model_plain: MMD
    value: 0.848
    std: 0.006
    paper_value: 0.848
    paper_std: 0.006
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
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.848
    true_std: 0.006
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.848
    sort_std: 0.006
    global_rank: 562
    paper_rank: 562
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRNN
    model_key: drnn
    model_plain: DRNN
    value: 0.771
    std: 0.012
    paper_value: 0.771
    paper_std: 0.012
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
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.771
    true_std: 0.012
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.771
    sort_std: 0.012
    global_rank: 598
    paper_rank: 598
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARM
    model_key: arm
    model_plain: ARM
    value: 0.746
    std: 0.007
    paper_value: 0.746
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
    protocol_note: Average accuracy across domains/runs as specified in the caption
      and text.
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    published_venue: TMLR 2026
    published_conference: TMLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.746
    true_std: 0.007
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.746
    sort_std: 0.007
    global_rank: 601
    paper_rank: 601
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
single_proposed_model: Graph-DG
main_figure: /figures/2602.05571/main_figure.jpegoptim.jpg
---

