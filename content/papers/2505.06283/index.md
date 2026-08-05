---
title: 'Soft causal learning for generalized molecule property prediction: An environment
  modeling perspective'
arxiv_id: '2505.06283'
source_url: ''
authors:
- name: Limin Li
  orcid: null
  s2_author_id: '2322605110'
  s2_url: null
- name: Zhen-Qiang Zhou
  orcid: null
  s2_author_id: '2278115693'
  s2_url: null
- name: Kuo Yang
  orcid: null
  s2_author_id: '2221673134'
  s2_url: null
- name: Wenjie Du
  orcid: null
  s2_author_id: '2188330082'
  s2_url: null
- name: Pengkun Wang
  orcid: null
  s2_author_id: '2108814780'
  s2_url: null
- name: Yang Wang
  orcid: null
  s2_author_id: '2186992833'
  s2_url: null
published_date: May 7, 2025
published_date_iso: '2025-05-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Learning on molecule graphs has become an increasingly important topic in
  AI for science, which takes full advantage of AI to facilitate scientific discovery.
  Existing solutions on modeling molecules utilize Graph Neural Networks (GNNs) to
  achieve representations, but they mostly fail to adapt models to out-of-distribution
  (OOD) samples. Although recent advances on OOD-oriented graph learning have discovered
  the invariant rationale on graphs, they still ignore three important issues, i.e.,
  1) the expanding atom patterns regarding environments on graphs lead to failures
  of invariant rationale-based models, 2) the associations between discovered molecular
  subgraphs and corresponding properties are complex where causal substructures cannot
  fully interpret the labels, and 3) the interactions between environments and invariances
  can influence with each other and thus are challenging to be modeled. To this end,
  we propose a soft causal learning framework, to tackle the unresolved molecule OOD
  challenge, from the perspective of negatively modeling the molecule environments
  and bypassing the invariant subgraphs. Specifically, we first incorporate chemistry
  theories into our graph growth generator to imitate expanded environments and then
  devise a GIB-based objective to disentangle environment from whole graphs and finally
  introduce a cross-attention-based soft causal interaction, which allows dynamic
  interactions between environments and invariances. We perform extensive experiments
  on seven datasets by imitating different kinds of OOD generalization scenarios.
  Extensive comparison, ablation experiments as well as visualized case studies demonstrate
  well generalization ability of our proposal.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CauEMO
mrr: 0.1166
adjusted_mrr: 0.1166
mrr_dataset_count: 3
benchmark_categories:
- TU Dortmund
- MoleculeNet
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 2
  total: 9
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: BBBP
  rows:
  - model: MAGPrompt+
    model_key: magprompt+
    model_plain: MAGPrompt+
    value: 0.9432
    std: 0.0238
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.05567'
    title: 'MAGPrompt: Message-Adaptive Graph Prompt Tuning for Graph Neural Networks'
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9432
    sort_std: 0.0238
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MAGPrompt+
    model_key: cams-llama
    model_plain: MAGPrompt+
    value: 0.942
    std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 100.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2601.02530'
    title: 'Multi-scale Graph Autoregressive Modeling: Molecular Property Prediction
      via Next Token Prediction'
    date: Jan 5, 2026
    date_display: Jan 2026
    date_iso: '2026-01-05'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.942
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MAGPrompt+
    model_key: se(3)-i mpph
    model_plain: MAGPrompt+
    value: 0.94
    std: 0.021
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_display: Dec 2023
    date_iso: '2023-12-12'
    venue: NeurIPS 2023 AI for Science Workshop
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: integrating SE(3)-invariance into Vietoris-Rips persistent
      homology
    is_global_top: true
    global_rank: 3
    sort_value: 0.94
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.6646
    std: 0.02
    paper_value: 0.6646
    paper_std: 0.02
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8875
    at_pub_std: 0.0049
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.2229
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8875
    true_std: 0.0049
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.2229
    has_value_note: false
    value_note: ''
    sort_value: 0.8875
    sort_std: 0.0049
    global_rank: 32
    paper_rank: 234
    rank_delta: 202
    rank_delta_abs: 202
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    comparison_source_arxiv: '2412.15589'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6534
    std: 0.0194
    paper_value: 0.6534
    paper_std: 0.0194
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.881
    at_pub_std: 0.036
    at_pub_source_arxiv: '2208.04529'
    at_pub_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    at_pub_source_date_iso: '2022-08-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-08-09'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.22760000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.881
    true_std: 0.036
    value_gap_source_arxiv: '2208.04529'
    value_gap_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    value_gap_source_is_current_paper: false
    value_gap: 0.22760000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.881
    sort_std: 0.036
    global_rank: 36
    paper_rank: 258
    rank_delta: 222
    rank_delta_abs: 222
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    comparison_source_arxiv: '2208.04529'
    is_best: false
    is_std_outlier: false
  - model: CauEMO
    model_key: cauemo
    model_plain: CauEMO
    value: 0.7231
    std: 0.0102
    paper_value: 0.7231
    paper_std: 0.0102
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7231
    true_std: 0.0102
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7231
    sort_std: 0.0102
    global_rank: 90
    paper_rank: 90
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.6913
    std: 0.0202
    paper_value: 0.6913
    paper_std: 0.0202
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6848
    at_pub_std: 0.0201
    at_pub_source_arxiv: '2312.10988'
    at_pub_source_title: Graph Invariant Learning with Subgraph Co-mixup for Out-Of-Distribution
      Generalization
    at_pub_source_date_iso: '2023-12-18'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2025-08-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.006500000000000061
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7155
    true_std: 0.0156
    value_gap_source_arxiv: '2508.17097'
    value_gap_source_title: 'Two Birds with One Stone: Enhancing Uncertainty Quantification
      and Interpretability with Graph Functional Neural Process'
    value_gap_source_is_current_paper: false
    value_gap: 0.0242
    has_value_note: false
    value_note: ''
    sort_value: 0.7155
    sort_std: 0.0156
    global_rank: 107
    paper_rank: 166
    rank_delta: 59
    rank_delta_abs: 59
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IGM
    model_key: igm
    model_plain: IGM
    value: 0.7103
    std: 0.0079
    paper_value: 0.7103
    paper_std: 0.0079
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7103
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2312.10988'
    at_pub_source_title: Graph Invariant Learning with Subgraph Co-mixup for Out-Of-Distribution
      Generalization
    at_pub_source_date_iso: '2023-12-18'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2023-12-18'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7103
    true_std: 0.0079
    value_gap_source_arxiv: '2312.10988'
    value_gap_source_title: Graph Invariant Learning with Subgraph Co-mixup for Out-Of-Distribution
      Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7103
    sort_std: 0.0079
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GALA
    model_key: gala
    model_plain: GALA
    value: 0.7021
    std: 0.0131
    paper_value: 0.7021
    paper_std: 0.0131
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7021
    true_std: 0.0131
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7021
    sort_std: 0.0131
    global_rank: 131
    paper_rank: 131
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.6973
    std: 0.0154
    paper_value: 0.6973
    paper_std: 0.0154
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6973
    at_pub_std: 0.0154
    at_pub_source_arxiv: '2312.10988'
    at_pub_source_title: Graph Invariant Learning with Subgraph Co-mixup for Out-Of-Distribution
      Generalization
    at_pub_source_date_iso: '2023-12-18'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2023-12-18'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6973
    true_std: 0.0154
    value_gap_source_arxiv: '2312.10988'
    value_gap_source_title: Graph Invariant Learning with Subgraph Co-mixup for Out-Of-Distribution
      Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6973
    sort_std: 0.0154
    global_rank: 151
    paper_rank: 151
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIGA
    model_key: ciga
    model_plain: CIGA
    value: 0.6965
    std: 0.0132
    paper_value: 0.6965
    paper_std: 0.0132
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6965
    at_pub_std: 0.0132
    at_pub_source_arxiv: '2312.10988'
    at_pub_source_title: Graph Invariant Learning with Subgraph Co-mixup for Out-Of-Distribution
      Generalization
    at_pub_source_date_iso: '2023-12-18'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2023-12-18'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6965
    true_std: 0.0132
    value_gap_source_arxiv: '2312.10988'
    value_gap_source_title: Graph Invariant Learning with Subgraph Co-mixup for Out-Of-Distribution
      Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6965
    sort_std: 0.0132
    global_rank: 157
    paper_rank: 157
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IB-Subgraph
    model_key: ib-subgraph
    model_plain: IB-Subgraph
    value: 0.6812
    std: 0.0112
    paper_value: 0.6812
    paper_std: 0.0112
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6812
    true_std: 0.0112
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6812
    sort_std: 0.0112
    global_rank: 189
    paper_rank: 189
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph-SAGE
    model_key: graph-sage
    model_plain: Graph-SAGE
    value: 0.6416
    std: 0.0283
    paper_value: 0.6416
    paper_std: 0.0283
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6416
    true_std: 0.0283
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6416
    sort_std: 0.0283
    global_rank: 273
    paper_rank: 273
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: MUTAG
  rows:
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
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
    input_feature_source: null
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
  - model: ECC
    model_key: supcosine
    model_plain: ECC
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
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CauEMO
    model_key: cauemo
    model_plain: CauEMO
    value: 0.9692
    std: 0.0136
    paper_value: 0.9692
    paper_std: 0.0136
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9692
    true_std: 0.0136
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9692
    sort_std: 0.0136
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
  - model: GALA
    model_key: gala
    model_plain: GALA
    value: 0.9676
    std: 0.017
    paper_value: 0.9676
    paper_std: 0.017
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9676
    true_std: 0.017
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9676
    sort_std: 0.017
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
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.9637
    std: 0.0215
    paper_value: 0.9637
    paper_std: 0.0215
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8088
    at_pub_std: 0.0894
    at_pub_source_arxiv: '2310.19906'
    at_pub_source_title: Interpretable Prototype-based Graph Information Bottleneck
    at_pub_source_date_iso: '2023-10-30'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.15490000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9637
    true_std: 0.0215
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9637
    sort_std: 0.0215
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Interpretable Prototype-based Graph Information Bottleneck
    comparison_source_arxiv: '2310.19906'
    is_best: false
    is_std_outlier: false
  - model: IGM
    model_key: igm
    model_plain: IGM
    value: 0.9604
    std: 0.0201
    paper_value: 0.9604
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9604
    true_std: 0.0201
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9604
    sort_std: 0.0201
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
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.9601
    std: 0.0224
    paper_value: 0.9601
    paper_std: 0.0224
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.895
    at_pub_std: 0.049
    at_pub_source_arxiv: '2303.14859'
    at_pub_source_title: Mind the Label Shift of Augmentation-based Graph OOD Generalization
    at_pub_source_date_iso: '2023-03-27'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.06509999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9601
    true_std: 0.0224
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9601
    sort_std: 0.0224
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIGA
    model_key: ciga
    model_plain: CIGA
    value: 0.9577
    std: 0.0123
    paper_value: 0.9577
    paper_std: 0.0123
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9577
    true_std: 0.0123
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9577
    sort_std: 0.0123
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
  - model: IB-Subgraph
    model_key: ib-subgraph
    model_plain: IB-Subgraph
    value: 0.9433
    std: 0.0644
    paper_value: 0.9433
    paper_std: 0.0644
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9433
    true_std: 0.0644
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9433
    sort_std: 0.0644
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8942
    std: 0.0563
    paper_value: 0.8942
    paper_std: 0.0563
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
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
    gap_vs_at_pub: 0.03880000000000006
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
    value_gap: 0.03880000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.029
    global_rank: 34
    paper_rank: 217
    rank_delta: 183
    rank_delta_abs: 183
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
    value: 0.8375
    std: 0.0474
    paper_value: 0.8375
    paper_std: 0.0474
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.922
    at_pub_std: 0.044
    at_pub_source_arxiv: '2503.01079'
    at_pub_source_title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery
      Curvature
    at_pub_source_date_iso: '2025-03-03'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2023-08-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.08450000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.891
    true_std: 0.058
    value_gap_source_arxiv: '2308.08235'
    value_gap_source_title: 'The Expressive Power of Graph Neural Networks: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.05349999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.891
    sort_std: 0.058
    global_rank: 250
    paper_rank: 500
    rank_delta: 250
    rank_delta_abs: 250
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph-SAGE
    model_key: graph-sage
    model_plain: Graph-SAGE
    value: 0.846
    std: 0.0534
    paper_value: 0.846
    paper_std: 0.0534
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
    protocol_note: 10-fold CV
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.846
    true_std: 0.0534
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.846
    sort_std: 0.0534
    global_rank: 455
    paper_rank: 455
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
- &id003
  dataset: SIDER
  rows:
  - model: DGI
    model_key: ka-gat
    model_plain: DGI
    value: 0.847
    std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.847
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DGI
    model_key: ka-gcn
    model_plain: DGI
    value: 0.842
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.842
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: graphkan
    model_plain: DGI
    value: 0.837
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.837
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.5624
    std: 0.0164
    paper_value: 0.5624
    paper_std: 0.0164
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6403
    at_pub_std: 0.0104
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.07789999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6403
    true_std: 0.0104
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.07789999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6403
    sort_std: 0.0104
    global_rank: 66
    paper_rank: 230
    rank_delta: 164
    rank_delta_abs: 164
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    comparison_source_arxiv: '2412.15589'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5212
    std: 0.0203
    paper_value: 0.5212
    paper_std: 0.0203
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.615
    at_pub_std: 0.025
    at_pub_source_arxiv: '2208.04529'
    at_pub_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    at_pub_source_date_iso: '2022-08-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-08-09'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0938
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.615
    true_std: 0.025
    value_gap_source_arxiv: '2208.04529'
    value_gap_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    value_gap_source_is_current_paper: false
    value_gap: 0.0938
    has_value_note: false
    value_note: ''
    sort_value: 0.615
    sort_std: 0.025
    global_rank: 127
    paper_rank: 241
    rank_delta: 114
    rank_delta_abs: 114
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    comparison_source_arxiv: '2208.04529'
    is_best: false
    is_std_outlier: false
  - model: CauEMO
    model_key: cauemo
    model_plain: CauEMO
    value: 0.599
    std: 0.0128
    paper_value: 0.599
    paper_std: 0.0128
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split; uses chemical knowledge-based environment generator
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.599
    true_std: 0.0128
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.599
    sort_std: 0.0128
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
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.5919
    std: 0.0103
    paper_value: 0.5919
    paper_std: 0.0103
    metric: ROC-AUC
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
    source_ref: miao2022interpretable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5758
    at_pub_std: 0.0123
    at_pub_source_arxiv: '2402.07191'
    at_pub_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    at_pub_source_date_iso: '2024-02-11'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.016100000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5919
    true_std: 0.0103
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5919
    sort_std: 0.0103
    global_rank: 202
    paper_rank: 202
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GALA
    model_key: gala
    model_plain: GALA
    value: 0.5904
    std: 0.013
    paper_value: 0.5904
    paper_std: 0.013
    metric: ROC-AUC
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
    source_ref: chen2023does
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5904
    true_std: 0.013
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5904
    sort_std: 0.013
    global_rank: 203
    paper_rank: 203
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIGA
    model_key: ciga
    model_plain: CIGA
    value: 0.5895
    std: 0.0122
    paper_value: 0.5895
    paper_std: 0.0122
    metric: ROC-AUC
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
    source_ref: chen2022learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5895
    true_std: 0.0122
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5895
    sort_std: 0.0122
    global_rank: 204
    paper_rank: 204
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.5881
    std: 0.0184
    paper_value: 0.5881
    paper_std: 0.0184
    metric: ROC-AUC
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
    source_ref: wu2022discovering
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5881
    true_std: 0.0184
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5881
    sort_std: 0.0184
    global_rank: 205
    paper_rank: 205
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IGM
    model_key: igm
    model_plain: IGM
    value: 0.5823
    std: 0.0143
    paper_value: 0.5823
    paper_std: 0.0143
    metric: ROC-AUC
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
    source_ref: jia2024graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5823
    true_std: 0.0143
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5823
    sort_std: 0.0143
    global_rank: 212
    paper_rank: 212
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IB-Subgraph
    model_key: ib-subgraph
    model_plain: IB-Subgraph
    value: 0.5771
    std: 0.0214
    paper_value: 0.5771
    paper_std: 0.0214
    metric: ROC-AUC
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
    source_ref: yu2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5771
    true_std: 0.0214
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5771
    sort_std: 0.0214
    global_rank: 216
    paper_rank: 216
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph-SAGE
    model_key: graph-sage
    model_plain: Graph-SAGE
    value: 0.5252
    std: 0.0169
    paper_value: 0.5252
    paper_std: 0.0169
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5252
    true_std: 0.0169
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5252
    sort_std: 0.0169
    global_rank: 241
    paper_rank: 241
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
- benchmark: MoleculeNet
  datasets:
  - *id002
  - *id003
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: BBBP
      dataset_slug: bbbp
    - dataset: SIDER
      dataset_slug: sider
single_proposed_model: CauEMO
main_figure: /figures/2505.06283/main_figure.jpegoptim.jpg
---

