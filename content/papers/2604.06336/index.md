---
title: 'BiScale-GTR: Fragment-Aware Graph Transformers for Multi-Scale Molecular Representation
  Learning'
arxiv_id: '2604.06336'
source_url: ''
authors:
- name: Yi Yang
  orcid: null
  s2_author_id: '2326649986'
  s2_url: null
- name: O. Daescu
  orcid: null
  s2_author_id: '2397728'
  s2_url: null
published_date: Apr 7, 2026
published_date_iso: '2026-04-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Transformers have recently attracted attention for molecular property
  prediction by combining the inductive biases of graph neural networks (GNNs) with
  the global receptive field of Transformers. However, many existing hybrid architectures
  remain GNN-dominated, causing the resulting representations to remain heavily shaped
  by local message passing. Moreover, most existing methods operate at only a single
  structural granularity, limiting their ability to capture molecular patterns that
  span multiple molecular scales. We introduce BiScale-GTR, a unified framework for
  self-supervised molecular representation learning that combines chemically grounded
  fragment tokenization with adaptive multi-scale reasoning. Our method improves graph
  Byte Pair Encoding (BPE) tokenization to produce consistent, chemically valid, and
  high-coverage fragment tokens, which are used as fragment-level inputs to a parallel
  GNN-Transformer architecture. Architecturally, atom-level representations learned
  by a GNN are pooled into fragment-level embeddings and fused with fragment token
  embeddings before Transformer reasoning, enabling the model to jointly capture local
  chemical environments, substructure-level motifs, and long-range molecular dependencies.
  Experiments on MoleculeNet, PharmaBench, and the Long Range Graph Benchmark (LRGB)
  demonstrate state-of-the-art performance across both classification and regression
  tasks. Attribution analysis further shows that BiScale-GTR highlights chemically
  meaningful functional motifs, providing interpretable links between molecular structure
  and predicted properties. Code will be released upon acceptance.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- BiScale-GTR (Molecule)
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 1
  total: 9
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ESOL
  rows:
  - model: KCL
    model_key: mat
    model_plain: KCL
    value: 0.278
    std: 0.02
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2002.08264'
    title: Molecule Attention Transformer
    date: Feb 19, 2020
    date_display: Feb 2020
    date_iso: '2020-02-19'
    venue: Graph Representation Learning workshop and Machine Learning and the Physical
      Sciences workshop at NeurIPS 2019
    codebase_url: https://github.com/gmum/MAT
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.278
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: KCL
    model_key: smiles
    model_plain: KCL
    value: 0.356
    std: 0.017
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2002.08264'
    title: Molecule Attention Transformer
    date: Feb 19, 2020
    date_display: Feb 2020
    date_iso: '2020-02-19'
    venue: Graph Representation Learning workshop and Machine Learning and the Physical
      Sciences workshop at NeurIPS 2019
    codebase_url: https://github.com/gmum/MAT
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.356
    sort_std: 0.017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KCL
    model_key: conan-fgw
    model_plain: KCL
    value: 0.514
    std: 0.019
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_display: Feb 2024
    date_iso: '2024-02-03'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.514
    sort_std: 0.019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FPGNN
    model_key: fpgnn
    model_plain: FPGNN
    value: 0.747
    std: null
    paper_value: 0.747
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.747
    sort_std: null
    global_rank: 32
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPG
    model_key: mpg
    model_plain: MPG
    value: 0.758
    std: null
    paper_value: 0.758
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.758
    sort_std: null
    global_rank: 32
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KANO
    model_key: kano
    model_plain: KANO
    value: 0.772
    std: null
    paper_value: 0.772
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.772
    sort_std: null
    global_rank: 33
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniMol
    model_key: unimol
    model_plain: UniMol
    value: 0.707
    std: null
    paper_value: 0.707
    paper_std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.788
    at_pub_std: 0.029
    at_pub_source_arxiv: '2402.01975'
    at_pub_source_title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation
      Networks
    at_pub_source_date_iso: '2024-02-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.08100000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.788
    true_std: 0.029
    value_gap_source_arxiv: '2402.01975'
    value_gap_source_title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08100000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: 0.029
    global_rank: 34
    paper_rank: 31
    rank_delta: -3
    rank_delta_abs: 3
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation
      Networks
    comparison_source_arxiv: '2402.01975'
    is_best: false
    is_std_outlier: false
  - model: DHTNN
    model_key: dhtnn
    model_plain: DHTNN
    value: 0.828
    std: null
    paper_value: 0.828
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.828
    sort_std: null
    global_rank: 42
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Trans-M
    model_key: trans-m
    model_plain: Trans-M
    value: 0.834
    std: null
    paper_value: 0.834
    paper_std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.834
    sort_std: null
    global_rank: 44
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CMPNN
    model_key: cmpnn
    model_plain: CMPNN
    value: 0.858
    std: null
    paper_value: 0.858
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.858
    sort_std: null
    global_rank: 46
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FragFormer
    model_key: fragformer
    model_plain: FragFormer
    value: 0.895
    std: null
    paper_value: 0.895
    paper_std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.895
    sort_std: null
    global_rank: 52
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PharmHGT
    model_key: pharmhgt
    model_plain: PharmHGT
    value: 0.954
    std: null
    paper_value: 0.954
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.954
    sort_std: null
    global_rank: 60
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BiScale-GTR (Molecule)
    model_key: biscale-gtr (molecule)
    model_plain: BiScale-GTR (Molecule)
    value: 0.977
    std: null
    paper_value: 0.977
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.977
    sort_std: null
    global_rank: 61
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: XGBoost
    model_key: xgboost
    model_plain: XGBoost
    value: 0.832
    std: null
    paper_value: 0.832
    paper_std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.99
    at_pub_std: 0.14
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.15800000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.99
    true_std: 0.14
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.15800000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.99
    sort_std: 0.14
    global_rank: 64
    paper_rank: 43
    rank_delta: -21
    rank_delta_abs: 21
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: MoleculeNet
    comparison_source_arxiv: '1703.00564'
    is_best: false
    is_std_outlier: false
  - model: rf
    model_key: rf
    model_plain: rf
    value: 0.918
    std: null
    paper_value: 0.918
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.07
    at_pub_std: 0.19
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.15200000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.07
    true_std: 0.19
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: false
    value_gap: 0.15200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 1.07
    sort_std: 0.19
    global_rank: 74
    paper_rank: 53
    rank_delta: -21
    rank_delta_abs: 21
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KP-GPT
    model_key: kp-gpt
    model_plain: KP-GPT
    value: 1.221
    std: null
    paper_value: 1.221
    paper_std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 1.221
    sort_std: null
    global_rank: 97
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FraGAT
    model_key: fragat
    model_plain: FraGAT
    value: 1.352
    std: null
    paper_value: 1.352
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 1.352
    sort_std: null
    global_rank: 100
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphFP
    model_key: graphfp
    model_plain: GraphFP
    value: 1.935
    std: null
    paper_value: 1.935
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    source_ref: niu2024pharmabench
    variant_inference_reason: 'dataset: fuzzy match to esol (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 7, 2026
    date_display: Apr 2026
    date_iso: '2026-04-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.136
    at_pub_std: 0.096
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.20100000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 2.136
    true_std: 0.096
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.20100000000000007
    has_value_note: false
    value_note: ''
    sort_value: 2.136
    sort_std: 0.096
    global_rank: 121
    paper_rank: 117
    rank_delta: -4
    rank_delta_abs: 4
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    comparison_source_arxiv: '2412.15589'
    is_best: false
    is_std_outlier: false
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
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
    - dataset: ESOL
      dataset_slug: esol
single_proposed_model: BiScale-GTR (Molecule)
main_figure: /figures/2604.06336/main_figure.jpegoptim.jpg
---

