---
title: 'ProtoMol: Enhancing Molecular Property Prediction via Prototype-Guided Multimodal
  Learning'
arxiv_id: '2510.16824'
source_url: ''
authors:
- name: Yingxu Wang
  orcid: null
  s2_author_id: '2374433961'
  s2_url: null
- name: Kunyu Zhang
  orcid: null
  s2_author_id: '2386632603'
  s2_url: null
- name: Jiaxing Huang
  orcid: null
  s2_author_id: '2340364119'
  s2_url: null
- name: Nan Yin
  orcid: null
  s2_author_id: '2331172981'
  s2_url: null
- name: Siwei Liu
  orcid: null
  s2_author_id: '2336874284'
  s2_url: null
- name: Eran Segal
  orcid: null
  s2_author_id: '2240562716'
  s2_url: null
published_date: Oct 19, 2025
published_date_iso: '2025-10-19'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Multimodal molecular representation learning, which jointly models molecular
  graphs and their textual descriptions, enhances predictive accuracy and interpretability
  by enabling more robust and reliable predictions of drug toxicity, bioactivity,
  and physicochemical properties through the integration of structural and semantic
  information. However, existing multimodal methods suffer from two key limitations:
  (1) they typically perform cross-modal interaction only at the final encoder layer,
  thus overlooking hierarchical semantic dependencies; (2) they lack a unified prototype
  space for robust alignment between modalities. To address these limitations, we
  propose ProtoMol, a prototype-guided multimodal framework that enables fine-grained
  integration and consistent semantic alignment between molecular graphs and textual
  descriptions. ProtoMol incorporates dual-branch hierarchical encoders, utilizing
  Graph Neural Networks to process structured molecular graphs and Transformers to
  encode unstructured texts, resulting in comprehensive layer-wise representations.
  Then, ProtoMol introduces a layer-wise bidirectional cross-modal attention mechanism
  that progressively aligns semantic features across layers. Furthermore, a shared
  prototype space with learnable, class-specific anchors is constructed to guide both
  modalities toward coherent and discriminative representations. Extensive experiments
  on multiple benchmark datasets demonstrate that ProtoMol consistently outperforms
  state-of-the-art baselines across a variety of molecular property prediction tasks.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ProtoMol
mrr: 1.0
adjusted_mrr: 0.3333
mrr_dataset_count: 1
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 1
  total: 9
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: BACE
  rows:
  - model: ProtoMol
    model_key: protomol
    model_plain: ProtoMol
    value: 0.914
    std: 0.003
    paper_value: 0.914
    paper_std: 0.003
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.914
    true_std: 0.003
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.914
    sort_std: 0.003
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
  - model: MMSG
    model_key: mmsg
    model_plain: MMSG
    value: 0.908
    std: 0.005
    paper_value: 0.908
    paper_std: 0.005
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.908
    true_std: 0.005
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.908
    sort_std: 0.005
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UnifiedMolPretrain
    model_key: memgnn
    model_plain: UnifiedMolPretrain
    value: 0.907
    std: 0.0
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.907
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tri_SGD
    model_key: tri_sgd
    model_plain: Tri_SGD
    value: 0.903
    std: 0.01
    paper_value: 0.903
    paper_std: 0.01
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.903
    true_std: 0.01
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: 0.01
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: S-CGIB
    model_key: s-cgib
    model_plain: S-CGIB
    value: 0.865
    std: 0.008
    paper_value: 0.865
    paper_std: 0.008
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8646
    at_pub_std: 0.0081
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.865
    true_std: 0.008
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.865
    sort_std: 0.008
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MDFCL
    model_key: mdfcl
    model_plain: MDFCL
    value: 0.864
    std: 0.01
    paper_value: 0.864
    paper_std: 0.01
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.864
    true_std: 0.01
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.864
    sort_std: 0.01
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Uni-Mol
    model_key: uni-mol
    model_plain: Uni-Mol
    value: 0.857
    std: 0.002
    paper_value: 0.857
    paper_std: 0.002
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.781
    at_pub_std: 0.014
    at_pub_source_arxiv: '2309.04589'
    at_pub_source_title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    at_pub_source_date_iso: '2023-09-08'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.07599999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.857
    true_std: 0.002
    value_gap_source_arxiv: '2604.16586'
    value_gap_source_title: A Systematic Survey and Benchmark of Deep Learning for
      Molecular Property Prediction in the Foundation Model Era
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.857
    sort_std: 0.002
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    comparison_source_arxiv: '2309.04589'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.743
    std: 0.014
    paper_value: 0.743
    paper_std: 0.014
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8451
    at_pub_std: null
    at_pub_source_arxiv: '2211.03666'
    at_pub_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    at_pub_source_date_iso: '2022-11-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.10209999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8451
    true_std: null
    value_gap_source_arxiv: '2211.03666'
    value_gap_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    value_gap_source_is_current_paper: false
    value_gap: 0.10209999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8451
    sort_std: null
    global_rank: 74
    paper_rank: 251
    rank_delta: 177
    rank_delta_abs: 177
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    comparison_source_arxiv: '2211.03666'
    is_best: false
    is_std_outlier: false
  - model: GraphLoG
    model_key: graphlog
    model_plain: GraphLoG
    value: 0.766
    std: 0.01
    paper_value: 0.766
    paper_std: 0.01
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.835
    at_pub_std: 0.012
    at_pub_source_arxiv: '2202.02989'
    at_pub_source_title: Graph Self-supervised Learning with Accurate Discrepancy
      Learning
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-22'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.06899999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.835
    true_std: 0.012
    value_gap_source_arxiv: '2205.10803'
    value_gap_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    value_gap_source_is_current_paper: false
    value_gap: 0.06899999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.835
    sort_std: 0.012
    global_rank: 91
    paper_rank: 233
    rank_delta: 142
    rank_delta_abs: 142
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Self-supervised Learning with Accurate Discrepancy
      Learning
    comparison_source_arxiv: '2202.02989'
    is_best: false
    is_std_outlier: false
  - model: SMILES-BERT
    model_key: smiles-bert
    model_plain: SMILES-BERT
    value: 0.833
    std: 0.033
    paper_value: 0.833
    paper_std: 0.033
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.833
    true_std: 0.033
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.833
    sort_std: 0.033
    global_rank: 96
    paper_rank: 96
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGSSL
    model_key: mgssl
    model_plain: MGSSL
    value: 0.82
    std: 0.038
    paper_value: 0.82
    paper_std: 0.038
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8203
    at_pub_std: 0.0379
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.000300000000000078
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8203
    true_std: 0.0379
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.000300000000000078
    has_value_note: false
    value_note: ''
    sort_value: 0.8203
    sort_std: 0.0379
    global_rank: 123
    paper_rank: 123
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MICRO-Graph
    model_key: micro-graph
    model_plain: MICRO-Graph
    value: 0.636
    std: 0.016
    paper_value: 0.636
    paper_std: 0.016
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.819
    at_pub_std: 0.004
    at_pub_source_arxiv: '2208.04529'
    at_pub_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    at_pub_source_date_iso: '2022-08-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-08-09'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.18299999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.819
    true_std: 0.004
    value_gap_source_arxiv: '2208.04529'
    value_gap_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    value_gap_source_is_current_paper: false
    value_gap: 0.18299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: 0.004
    global_rank: 126
    paper_rank: 300
    rank_delta: 174
    rank_delta_abs: 174
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    comparison_source_arxiv: '2208.04529'
    is_best: false
    is_std_outlier: false
  - model: SMILES2vec
    model_key: smiles2vec
    model_plain: SMILES2vec
    value: 0.814
    std: 0.036
    paper_value: 0.814
    paper_std: 0.036
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.814
    true_std: 0.036
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.814
    sort_std: 0.036
    global_rank: 138
    paper_rank: 138
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoAMa
    model_key: moama
    model_plain: MoAMa
    value: 0.813
    std: 0.011
    paper_value: 0.813
    paper_std: 0.011
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8132
    at_pub_std: 0.0106
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.000200000000000089
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8132
    true_std: 0.0106
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.000200000000000089
    has_value_note: false
    value_note: ''
    sort_value: 0.8132
    sort_std: 0.0106
    global_rank: 140
    paper_rank: 140
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GROVE
    model_key: grove
    model_plain: GROVE
    value: 0.811
    std: 0.001
    paper_value: 0.811
    paper_std: 0.001
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8113
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8113
    true_std: 0.0014
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.8113
    sort_std: 0.0014
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphFP
    model_key: graphfp
    model_plain: GraphFP
    value: 0.803
    std: 0.031
    paper_value: 0.803
    paper_std: 0.031
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8028
    at_pub_std: 0.0306
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.000200000000000089
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.803
    true_std: 0.031
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.803
    sort_std: 0.031
    global_rank: 165
    paper_rank: 165
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimSGT
    model_key: simsgt
    model_plain: SimSGT
    value: 0.798
    std: 0.013
    paper_value: 0.798
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7975
    at_pub_std: 0.0128
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.000500000000000056
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.798
    true_std: 0.013
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.798
    sort_std: 0.013
    global_rank: 173
    paper_rank: 173
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.778
    std: 0.005
    paper_value: 0.778
    paper_std: 0.005
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.782
    at_pub_std: 0.012
    at_pub_source_arxiv: '2205.15746'
    at_pub_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    at_pub_source_date_iso: '2022-05-31'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.782
    true_std: 0.012
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.012
    global_rank: 210
    paper_rank: 219
    rank_delta: 9
    rank_delta_abs: 9
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
    value: 0.778
    std: 0.005
    paper_value: 0.778
    paper_std: 0.005
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.759
    at_pub_std: 0.016
    at_pub_source_arxiv: '2309.02304'
    at_pub_source_title: Graph Self-Contrast Representation Learning
    at_pub_source_date_iso: '2023-09-05'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.019000000000000017
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.778
    true_std: 0.005
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.005
    global_rank: 221
    paper_rank: 221
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphPT
    model_key: graphpt
    model_plain: GraphPT
    value: 0.76
    std: 0.005
    paper_value: 0.76
    paper_std: 0.005
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.76
    true_std: 0.005
    value_gap_source_arxiv: '2510.16824'
    value_gap_source_title: 'ProtoMol: Enhancing Molecular Property Prediction via
      Prototype-Guided Multimodal Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.005
    global_rank: 238
    paper_rank: 238
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.744
    std: 0.017
    paper_value: 0.744
    paper_std: 0.017
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
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7549
    at_pub_std: 0.0127
    at_pub_source_arxiv: '2106.05819'
    at_pub_source_title: Adversarial Graph Augmentation to Improve Graph Contrastive
      Learning
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2021-06-10'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.01090000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7549
    true_std: 0.0127
    value_gap_source_arxiv: '2106.05819'
    value_gap_source_title: Adversarial Graph Augmentation to Improve Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.01090000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7549
    sort_std: 0.0127
    global_rank: 242
    paper_rank: 250
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
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
- benchmark: MoleculeNet
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: BACE
      dataset_slug: bace
single_proposed_model: ProtoMol
---

