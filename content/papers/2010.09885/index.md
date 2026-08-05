---
title: 'ChemBERTa: Large-Scale Self-Supervised Pretraining for Molecular Property
  Prediction'
arxiv_id: '2010.09885'
source_url: ''
authors:
- name: Seyone Chithrananda
  orcid: null
  s2_author_id: '1999563324'
  s2_url: null
- name: Gabriel Grand
  orcid: null
  s2_author_id: '35748708'
  s2_url: null
- name: Bharath Ramsundar
  orcid: null
  s2_author_id: '2378027'
  s2_url: null
published_date: Oct 19, 2020
published_date_iso: '2020-10-19'
published_venue: NeurIPS 2020
published_conference: NeurIPS 2020
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: GNNs and chemical fingerprints are the predominant approaches to representing
  molecules for property prediction. However, in NLP, transformers have become the
  de-facto standard for representation learning thanks to their strong downstream
  task transfer. In parallel, the software ecosystem around transformers is maturing
  rapidly, with libraries like HuggingFace and BertViz enabling streamlined training
  and introspection. In this work, we make one of the first attempts to systematically
  evaluate transformers on molecular property prediction tasks via our ChemBERTa model.
  While not at state-of-the-art, ChemBERTa scales well with pretraining dataset size,
  offering competitive downstream performance on MoleculeNet and useful attention-based
  visualization modalities. Our results suggest that transformers offer a promising
  avenue of future work for molecular representation learning and property prediction.
  To facilitate these efforts, we release a curated dataset of 77M SMILES from PubChem
  suitable for large-scale self-supervised pretraining.
codebase_url: https://huggingface.co/seyonec/ChemBERTa-zinc-base-v1
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ChemBERTa 10M
mrr: 0.0036
adjusted_mrr: 0.0012
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
  - model: CamS-LLaMA
    model_key: cams-llama
    model_plain: CamS-LLaMA
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
  - model: SE(3)-I MPPH
    model_key: se(3)-i mpph
    model_plain: SE(3)-I MPPH
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
  - model: D-MPNN
    model_key: d-mpnn
    model_plain: D-MPNN
    value: 0.708
    std: null
    paper_value: 0.708
    paper_std: null
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
    source_ref: Chemprop
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 80/10/10 scaffold split using DeepChem
    date: Oct 19, 2020
    date_display: Oct 2020
    date_iso: '2020-10-19'
    published_venue: NeurIPS 2020
    published_conference: NeurIPS 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.913
    true_std: 0.026
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.20500000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.913
    sort_std: 0.026
    global_rank: 25
    paper_rank: 120
    rank_delta: 95
    rank_delta_abs: 95
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8875
    std: 0.0049
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.15589'
    title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
      Graph Information Bottleneck
    date: Dec 20, 2024
    date_display: Dec 2024
    date_iso: '2024-12-20'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/NSLab-CUK/S-CGIB
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 32
    sort_value: 0.8875
    sort_std: 0.0049
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: rf
    model_key: rf
    model_plain: rf
    value: 0.681
    std: null
    paper_value: 0.681
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Chemprop
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 80/10/10 scaffold split using DeepChem
    date: Oct 19, 2020
    date_display: Oct 2020
    date_iso: '2020-10-19'
    published_venue: NeurIPS 2020
    published_conference: NeurIPS 2020
    at_pub_value: 0.725
    at_pub_std: 0.006
    at_pub_source_arxiv: '2002.08264'
    at_pub_source_title: Molecule Attention Transformer
    at_pub_source_date_iso: '2020-02-19'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-02-19'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.04399999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.725
    true_std: 0.006
    value_gap_source_arxiv: '2002.08264'
    value_gap_source_title: Molecule Attention Transformer
    value_gap_source_is_current_paper: false
    value_gap: 0.04399999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.725
    sort_std: 0.006
    global_rank: 88
    paper_rank: 195
    rank_delta: 107
    rank_delta_abs: 107
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecule Attention Transformer
    comparison_source_arxiv: '2002.08264'
    is_best: false
    is_std_outlier: false
  - model: SVM
    model_key: svm
    model_plain: SVM
    value: 0.702
    std: null
    paper_value: 0.702
    paper_std: null
    metric: ROC-AUC
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
    source_ref: Chemprop
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 80/10/10 scaffold split using DeepChem
    date: Oct 19, 2020
    date_display: Oct 2020
    date_iso: '2020-10-19'
    published_venue: NeurIPS 2020
    published_conference: NeurIPS 2020
    at_pub_value: 0.723
    at_pub_std: 0.0
    at_pub_source_arxiv: '2002.08264'
    at_pub_source_title: Molecule Attention Transformer
    at_pub_source_date_iso: '2020-02-19'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-02-19'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.02100000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.723
    true_std: 0.0
    value_gap_source_arxiv: '2002.08264'
    value_gap_source_title: Molecule Attention Transformer
    value_gap_source_is_current_paper: false
    value_gap: 0.02100000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.723
    sort_std: 0.0
    global_rank: 94
    paper_rank: 136
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecule Attention Transformer
    comparison_source_arxiv: '2002.08264'
    is_best: false
    is_std_outlier: false
  - model: ChemBERTa 10M
    model_key: chemberta 10m
    model_plain: ChemBERTa 10M
    value: 0.643
    std: null
    paper_value: 0.643
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 80/10/10 scaffold split using DeepChem
    date: Oct 19, 2020
    date_display: Oct 2020
    date_iso: '2020-10-19'
    published_venue: NeurIPS 2020
    published_conference: NeurIPS 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-19'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.643
    true_std: null
    value_gap_source_arxiv: '2010.09885'
    value_gap_source_title: 'ChemBERTa: Large-Scale Self-Supervised Pretraining for
      Molecular Property Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.643
    sort_std: null
    global_rank: 277
    paper_rank: 277
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
    - dataset: BBBP
      dataset_slug: bbbp
single_proposed_model: ChemBERTa 10M
main_figure: /figures/2010.09885/main_figure.jpegoptim.jpg
---

