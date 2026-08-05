---
title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation'
arxiv_id: '2502.12638'
source_url: ''
authors:
- name: Zhiyuan Liu
  orcid: null
  s2_author_id: '2322351492'
  s2_url: null
- name: Yanchen Luo
  orcid: null
  s2_author_id: '2231664238'
  s2_url: null
- name: Han Huang
  orcid: null
  s2_author_id: '2143496455'
  s2_url: null
- name: Enzhi Zhang
  orcid: null
  s2_author_id: '2261086256'
  s2_url: null
- name: Sihang Li
  orcid: null
  s2_author_id: '2261249035'
  s2_url: null
- name: Junfeng Fang
  orcid: null
  s2_author_id: '2322305642'
  s2_url: null
- name: Yaorui Shi
  orcid: null
  s2_author_id: '2261094053'
  s2_url: null
- name: Xiang Wang
  orcid: null
  s2_author_id: '2260296919'
  s2_url: null
- name: Kenji Kawaguchi
  orcid: null
  s2_author_id: '2260546802'
  s2_url: null
- name: Tat-Seng Chua
  orcid: null
  s2_author_id: '2257036129'
  s2_url: null
published_date: Feb 18, 2025
published_date_iso: '2025-02-18'
published_venue: ICLR 2025
published_conference: ICLR 2025
published_conference_short: ICLR
published_conference_slug: iclr
abstract: '3D molecule generation is crucial for drug discovery and material design.
  While prior efforts focus on 3D diffusion models for their benefits in modeling
  continuous 3D conformers, they overlook the advantages of 1D SELFIES-based Language
  Models (LMs), which can generate 100% valid molecules and leverage the billion-scale
  1D molecule datasets. To combine these advantages for 3D molecule generation, we
  propose a foundation model -- NExT-Mol: 3D Diffusion Meets 1D Language Modeling
  for 3D Molecule Generation. NExT-Mol uses an extensively pretrained molecule LM
  for 1D molecule generation, and subsequently predicts the generated molecule''s
  3D conformers with a 3D diffusion model. We enhance NExT-Mol''s performance by scaling
  up the LM''s model size, refining the diffusion neural architecture, and applying
  1D to 3D transfer learning. Notably, our 1D molecule LM significantly outperforms
  baselines in distributional similarity while ensuring validity, and our 3D diffusion
  model achieves leading performances in conformer prediction. Given these improvements
  in 1D and 3D modeling, NExT-Mol achieves a 26% relative improvement in 3D FCD for
  de novo 3D generation on GEOM-DRUGS, and a 13% average relative gain for conditional
  3D generation on QM9-2014. Our codes and pretrained checkpoints are available at
  https://github.com/acharkq/NExT-Mol.'
codebase_url: https://github.com/acharkq/NExT-Mol
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- MoleculeNet
- Quantum Chemistry
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 2
  total: 9
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 1
  total: 3
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ESOL
  rows:
  - model: AMCT
    model_key: mat
    model_plain: AMCT
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
  - model: AMCT
    model_key: smiles
    model_plain: AMCT
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
  - model: AMCT
    model_key: graphormer-spis
    model_plain: AMCT
    value: 0.484
    std: 0.005
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_display: May 2023
    date_iso: '2023-05-23'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.484
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 1.43
    std: 0.05
    paper_value: 1.43
    paper_std: 0.05
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kipf2017semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.564
    at_pub_std: 0.015
    at_pub_source_arxiv: '2305.13987'
    at_pub_source_title: On Structural Expressive Power of Graph Transformers
    at_pub_source_date_iso: '2023-05-23'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-05-23'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.866
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.564
    true_std: 0.015
    value_gap_source_arxiv: '2305.13987'
    value_gap_source_title: On Structural Expressive Power of Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.866
    has_value_note: false
    value_note: ''
    sort_value: 0.564
    sort_std: 0.015
    global_rank: 9
    paper_rank: 114
    rank_delta: 105
    rank_delta_abs: 105
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Structural Expressive Power of Graph Transformers
    comparison_source_arxiv: '2305.13987'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 1.45
    std: 0.02
    paper_value: 1.45
    paper_std: 0.02
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: xu2019powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.626
    at_pub_std: 0.017
    at_pub_source_arxiv: '2305.13987'
    at_pub_source_title: On Structural Expressive Power of Graph Transformers
    at_pub_source_date_iso: '2023-05-23'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-05-23'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.824
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.626
    true_std: 0.017
    value_gap_source_arxiv: '2305.13987'
    value_gap_source_title: On Structural Expressive Power of Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.824
    has_value_note: false
    value_note: ''
    sort_value: 0.626
    sort_std: 0.017
    global_rank: 26
    paper_rank: 114
    rank_delta: 88
    rank_delta_abs: 88
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Structural Expressive Power of Graph Transformers
    comparison_source_arxiv: '2305.13987'
    is_best: false
    is_std_outlier: false
  - model: D-MPNN
    model_key: d-mpnn
    model_plain: D-MPNN
    value: 0.98
    std: 0.26
    paper_value: 0.98
    paper_std: 0.26
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: D-MPNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.635
    at_pub_std: 0.027
    at_pub_source_arxiv: '2006.04804'
    at_pub_source_title: Optimal Transport Graph Neural Networks
    at_pub_source_date_iso: '2020-06-08'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-08'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.345
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.635
    true_std: 0.027
    value_gap_source_arxiv: '2006.04804'
    value_gap_source_title: Optimal Transport Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.345
    has_value_note: false
    value_note: ''
    sort_value: 0.635
    sort_std: 0.027
    global_rank: 28
    paper_rank: 70
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Optimal Transport Graph Neural Networks
    comparison_source_arxiv: '2006.04804'
    is_best: false
    is_std_outlier: false
  - model: MoLlama
    model_key: mollama
    model_plain: MoLlama
    value: 0.74
    std: 0.01
    paper_value: 0.74
    paper_std: 0.01
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: pretrain MoLlama on a large collection of 1.8B SELFIES
      sequences
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.74
    true_std: 0.01
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.74
    sort_std: 0.01
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolPROP
    model_key: molprop
    model_plain: MolPROP
    value: 0.777
    std: 0.02
    paper_value: 0.777
    paper_std: 0.02
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: LM-based Methods
    table_ref: Table 1
    source_ref: MolPROP
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.777
    true_std: 0.02
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.777
    sort_std: 0.02
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
  - model: ChemBERTa-2
    model_key: chemberta-2
    model_plain: ChemBERTa-2
    value: 0.889
    std: 0.0
    paper_value: 0.889
    paper_std: 0.0
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: LM-based Methods
    table_ref: Table 1
    source_ref: chemberta-2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.889
    at_pub_std: null
    at_pub_source_arxiv: '2402.01975'
    at_pub_source_title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation
      Networks
    at_pub_source_date_iso: '2024-02-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.889
    true_std: 0.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.889
    sort_std: 0.0
    global_rank: 58
    paper_rank: 58
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3D Infomax
    model_key: 3d infomax
    model_plain: 3D Infomax
    value: 0.95
    std: 0.04
    paper_value: 0.95
    paper_std: 0.04
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.894
    at_pub_std: 0.028
    at_pub_source_arxiv: '2110.04126'
    at_pub_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    at_pub_source_date_iso: '2021-10-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: 0.05599999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.894
    true_std: 0.028
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.05599999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: 0.028
    global_rank: 59
    paper_rank: 69
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 1.05
    std: 0.06
    paper_value: 1.05
    paper_std: 0.06
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: schutt2018schnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 1.045
    at_pub_std: 0.064
    at_pub_source_arxiv: '2310.07351'
    at_pub_source_title: Atom-Motif Contrastive Transformer for Molecular Property
      Prediction
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.0050000000000001155
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 1.045
    true_std: 0.064
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.0050000000000001155
    has_value_note: false
    value_note: ''
    sort_value: 1.045
    sort_std: 0.064
    global_rank: 79
    paper_rank: 80
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: rf
    model_key: rf
    model_plain: rf
    value: 1.07
    std: 0.19
    paper_value: 1.07
    paper_std: 0.19
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MolCLR
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 1.07
    at_pub_std: 0.19
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.07
    true_std: 0.19
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.07
    sort_std: 0.19
    global_rank: 84
    paper_rank: 84
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolCLR
    model_key: molclr
    model_plain: MolCLR
    value: 1.11
    std: 0.01
    paper_value: 1.11
    paper_std: 0.01
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: Pretrained GNN-based Methods
    table_ref: Table 1
    source_ref: MolCLR
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 1.11
    at_pub_std: 0.01
    at_pub_source_arxiv: '2202.09346'
    at_pub_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.11
    true_std: 0.01
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.11
    sort_std: 0.01
    global_rank: 93
    paper_rank: 93
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Pretrain-GNN
    model_key: pretrain-gnn
    model_plain: Pretrain-GNN
    value: 1.22
    std: 0.02
    paper_value: 1.22
    paper_std: 0.02
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: Pretrained GNN-based Methods
    table_ref: Table 1
    source_ref: pretrain_gnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.22
    true_std: 0.02
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.22
    sort_std: 0.02
    global_rank: 107
    paper_rank: 107
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 1.27
    std: 0.15
    paper_value: 1.27
    paper_std: 0.15
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MGCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 1.266
    at_pub_std: 0.147
    at_pub_source_arxiv: '2310.07351'
    at_pub_source_title: Atom-Motif Contrastive Transformer for Molecular Property
      Prediction
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 1.266
    true_std: 0.147
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 1.266
    sort_std: 0.147
    global_rank: 109
    paper_rank: 109
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 1.41
    std: 0.0
    paper_value: 1.41
    paper_std: 0.0
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: GATv2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.41
    true_std: 0.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.41
    sort_std: 0.0
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
  - model: SVM
    model_key: svm
    model_plain: SVM
    value: 1.5
    std: 0.0
    paper_value: 1.5
    paper_std: 0.0
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MolCLR
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.5
    true_std: 0.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.5
    sort_std: 0.0
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
- &id002
  dataset: FreeSolv
  rows:
  - model: D&D-Node +vn
    model_key: se(3)-i mpph
    model_plain: D&D-Node +vn
    value: 0.354
    std: 0.053
    metric: RMSE
    higher_is_better: false
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
    global_rank: 1
    sort_value: 0.354
    sort_std: 0.053
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: ecfp-4 + rf
    model_plain: D&D-Node +vn
    value: 0.56
    std: 0.066
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
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
    feature_source_evidence: trained on ECFP-4 fingerprints
    is_global_top: true
    global_rank: 2
    sort_value: 0.56
    sort_std: 0.066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: geomgcl
    model_plain: D&D-Node +vn
    value: 0.866
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_display: Sep 2021
    date_iso: '2021-09-24'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: The model uses a 2D-3D geometric contrastive scheme to
      bridge knowledge between 2D chemical semantics and 3D spatial information.
    is_global_top: true
    global_rank: 3
    sort_value: 0.866
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D-MPNN
    model_key: d-mpnn
    model_plain: D-MPNN
    value: 2.18
    std: 0.91
    paper_value: 2.18
    paper_std: 0.91
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: D-MPNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 1.01
    at_pub_std: 0.064
    at_pub_source_arxiv: '2312.07633'
    at_pub_source_title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    at_pub_source_date_iso: '2023-12-12'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 1.1700000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 1.01
    true_std: 0.064
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 1.1700000000000002
    has_value_note: false
    value_note: ''
    sort_value: 1.01
    sort_std: 0.064
    global_rank: 8
    paper_rank: 45
    rank_delta: 37
    rank_delta_abs: 37
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    comparison_source_arxiv: '2312.07633'
    is_best: false
    is_std_outlier: false
  - model: MoLlama
    model_key: mollama
    model_plain: MoLlama
    value: 1.59
    std: 0.04
    paper_value: 1.59
    paper_std: 0.04
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: MoLlama is a 960M parameter LM... pretrain it from scratch...
      extensive pretraining empowers MoLlama to effectively capture the desired 1D/2D
      molecular patterns
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.59
    true_std: 0.04
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.59
    sort_std: 0.04
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
  - model: MolPROP
    model_key: molprop
    model_plain: MolPROP
    value: 1.7
    std: 0.09
    paper_value: 1.7
    paper_std: 0.09
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: LM-based Methods
    table_ref: Table 1
    source_ref: MolPROP
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.7
    true_std: 0.09
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.7
    sort_std: 0.09
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: rf
    model_key: rf
    model_plain: rf
    value: 2.03
    std: 0.22
    paper_value: 2.03
    paper_std: 0.22
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MolCLR
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 2.03
    at_pub_std: 0.22
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.03
    true_std: 0.22
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.03
    sort_std: 0.22
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChemBERTa-2
    model_key: chemberta-2
    model_plain: ChemBERTa-2
    value: 2.047
    std: 0.0
    paper_value: 2.047
    paper_std: 0.0
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: LM-based Methods
    table_ref: Table 1
    source_ref: chemberta-2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.047
    true_std: 0.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.047
    sort_std: 0.0
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
  - model: MolCLR
    model_key: molclr
    model_plain: MolCLR
    value: 2.2
    std: 0.2
    paper_value: 2.2
    paper_std: 0.2
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MolCLR
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 2.2
    at_pub_std: 0.2
    at_pub_source_arxiv: '2202.09346'
    at_pub_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.2
    true_std: 0.2
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.2
    sort_std: 0.2
    global_rank: 49
    paper_rank: 49
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3D Infomax
    model_key: 3d infomax
    model_plain: 3D Infomax
    value: 2.23
    std: 0.26
    paper_value: 2.23
    paper_std: 0.26
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 2.337
    at_pub_std: 0.227
    at_pub_source_arxiv: '2110.04126'
    at_pub_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    at_pub_source_date_iso: '2021-10-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.1070000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.23
    true_std: 0.26
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.23
    sort_std: 0.26
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 2.76
    std: 0.18
    paper_value: 2.76
    paper_std: 0.18
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: xu2019powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 2.346
    at_pub_std: 0.122
    at_pub_source_arxiv: '2106.06130'
    at_pub_source_title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning
      for Property Prediction'
    at_pub_source_date_iso: '2021-06-11'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-06-11'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.4139999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 2.346
    true_std: 0.122
    value_gap_source_arxiv: '2106.06130'
    value_gap_source_title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation
      Learning for Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.4139999999999997
    has_value_note: false
    value_note: ''
    sort_value: 2.346
    sort_std: 0.122
    global_rank: 56
    paper_rank: 72
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation
      Learning for Property Prediction'
    comparison_source_arxiv: '2106.06130'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 2.87
    std: 0.14
    paper_value: 2.87
    paper_std: 0.14
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kipf2017semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 2.618
    at_pub_std: 0.298
    at_pub_source_arxiv: '2310.16401'
    at_pub_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.2520000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 2.618
    true_std: 0.298
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.2520000000000002
    has_value_note: false
    value_note: ''
    sort_value: 2.618
    sort_std: 0.298
    global_rank: 66
    paper_rank: 78
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Pretrain-GNN
    model_key: pretrain-gnn
    model_plain: Pretrain-GNN
    value: 2.83
    std: 0.12
    paper_value: 2.83
    paper_std: 0.12
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: pretrain_gnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.83
    true_std: 0.12
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.83
    sort_std: 0.12
    global_rank: 77
    paper_rank: 77
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SVM
    model_key: svm
    model_plain: SVM
    value: 3.14
    std: 0.0
    paper_value: 3.14
    paper_std: 0.0
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MolCLR
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.14
    true_std: 0.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.14
    sort_std: 0.0
    global_rank: 89
    paper_rank: 89
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 3.14
    std: 0.0
    paper_value: 3.14
    paper_std: 0.0
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: GATv2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.14
    true_std: 0.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.14
    sort_std: 0.0
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
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 3.22
    std: 0.76
    paper_value: 3.22
    paper_std: 0.76
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: schutt2018schnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 3.215
    at_pub_std: 0.755
    at_pub_source_arxiv: '2312.07633'
    at_pub_source_title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    at_pub_source_date_iso: '2023-12-12'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.0050000000000003375
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 3.215
    true_std: 0.755
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.0050000000000003375
    has_value_note: false
    value_note: ''
    sort_value: 3.215
    sort_std: 0.755
    global_rank: 93
    paper_rank: 93
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 3.35
    std: 0.01
    paper_value: 3.35
    paper_std: 0.01
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MGCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 3.349
    at_pub_std: 0.097
    at_pub_source_arxiv: '2312.07633'
    at_pub_source_title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    at_pub_source_date_iso: '2023-12-12'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.0009999999999998899
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 3.349
    true_std: 0.097
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.0009999999999998899
    has_value_note: false
    value_note: ''
    sort_value: 3.349
    sort_std: 0.097
    global_rank: 96
    paper_rank: 96
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
- &id003
  dataset: QM7b
  rows:
  - model: ISGR
    model_key: ani-1
    model_plain: ISGR
    value: 2.86
    std: 0.25
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1907.04786'
    title: Fast Haar Transforms for Graph Neural Networks
    date: Jul 10, 2019
    date_display: Jul 2019
    date_iso: '2019-07-10'
    venue: Neural Networks
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 2.86
    sort_std: 0.25
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ISGR
    model_key: dtnn
    model_plain: ISGR
    value: 8.8
    std: 3.5
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1907.04786'
    title: Fast Haar Transforms for Graph Neural Networks
    date: Jul 10, 2019
    date_display: Jul 2019
    date_iso: '2019-07-10'
    venue: Neural Networks
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 8.8
    sort_std: 3.5
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ISGR
    model_key: hanet
    model_plain: ISGR
    value: 9.5
    std: 0.71
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1907.04786'
    title: Fast Haar Transforms for Graph Neural Networks
    date: Jul 10, 2019
    date_display: Jul 2019
    date_iso: '2019-07-10'
    venue: Neural Networks
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 9.5
    sort_std: 0.71
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoLlama
    model_key: mollama
    model_plain: MoLlama
    value: 63.5
    std: 1.6
    paper_value: 63.5
    paper_std: 1.6
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: pretrain MoLlama ... on a large collection of 1.8B SELFIES
      sequences
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 63.5
    true_std: 1.6
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 63.5
    sort_std: 1.6
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
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 74.2
    std: 6.0
    paper_value: 74.2
    paper_std: 6.0
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: schutt2018schnet
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 74.2
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 74.2
    true_std: 6.0
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 74.2
    sort_std: 6.0
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
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 77.6
    std: 4.7
    paper_value: 77.6
    paper_std: 4.7
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MGCN
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 77.6
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 77.6
    true_std: 4.7
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 77.6
    sort_std: 4.7
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
    is_std_outlier: false
  - model: MolCLR
    model_key: molclr
    model_plain: MolCLR
    value: 87.2
    std: 2.0
    paper_value: 87.2
    paper_std: 2.0
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MolCLR
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 87.2
    at_pub_std: 2.0
    at_pub_source_arxiv: '2202.09346'
    at_pub_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 87.2
    true_std: 2.0
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 87.2
    sort_std: 2.0
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D-MPNN
    model_key: d-mpnn
    model_plain: D-MPNN
    value: 105.8
    std: 13.2
    paper_value: 105.8
    paper_std: 13.2
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: D-MPNN
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 105.8
    at_pub_std: 13.2
    at_pub_source_arxiv: '2202.09346'
    at_pub_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 105.8
    true_std: 13.2
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 105.8
    sort_std: 13.2
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Pretrain-GNN
    model_key: pretrain-gnn
    model_plain: Pretrain-GNN
    value: 110.2
    std: 6.4
    paper_value: 110.2
    paper_std: 6.4
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: pretrain_gnn
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 110.2
    true_std: 6.4
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 110.2
    sort_std: 6.4
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 113.3
    std: 0.0
    paper_value: 113.3
    paper_std: 0.0
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: GATv2
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 113.3
    true_std: 0.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 113.3
    sort_std: 0.0
    global_rank: 35
    paper_rank: 35
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: rf
    model_key: rf
    model_plain: rf
    value: 122.7
    std: 4.2
    paper_value: 122.7
    paper_std: 4.2
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MolCLR
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 122.7
    at_pub_std: 4.2
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2019-07-10'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 122.7
    true_std: 4.2
    value_gap_source_arxiv: '1907.04786'
    value_gap_source_title: Fast Haar Transforms for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 122.7
    sort_std: 4.2
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 122.9
    std: 2.2
    paper_value: 122.9
    paper_std: 2.2
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kipf2017semi
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 122.9
    at_pub_std: 2.2
    at_pub_source_arxiv: '2202.09346'
    at_pub_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 122.9
    true_std: 2.2
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 122.9
    sort_std: 2.2
    global_rank: 38
    paper_rank: 38
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
    value: 124.8
    std: 0.7
    paper_value: 124.8
    paper_std: 0.7
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: xu2019powerful
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 124.8
    at_pub_std: 0.7
    at_pub_source_arxiv: '2202.09346'
    at_pub_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 124.8
    true_std: 0.7
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 124.8
    sort_std: 0.7
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
  - model: MolPROP
    model_key: molprop
    model_plain: MolPROP
    value: 151.8
    std: 10.0
    paper_value: 151.8
    paper_std: 10.0
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MolPROP
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 151.8
    true_std: 10.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 151.8
    sort_std: 10.0
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
  - model: SVM
    model_key: svm
    model_plain: SVM
    value: 156.9
    std: 0.0
    paper_value: 156.9
    paper_std: 0.0
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: MolCLR
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 156.9
    true_std: 0.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 156.9
    sort_std: 0.0
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChemBERTa-2
    model_key: chemberta-2
    model_plain: ChemBERTa-2
    value: 172.8
    std: 0.0
    paper_value: 172.8
    paper_std: 0.0
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chemberta-2
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MoleculeNet QM7 split as per MolPROP
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-18'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 172.8
    true_std: 0.0
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 172.8
    sort_std: 0.0
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: MoleculeNet
  datasets:
  - *id001
  - *id002
- benchmark: Quantum Chemistry
  datasets:
  - *id003
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: ESOL
      dataset_slug: esol
    - dataset: FreeSolv
      dataset_slug: freesolv
  - benchmark: Quantum Chemistry
    benchmark_slug: quantum-chemistry
    datasets:
    - dataset: QM7b
      dataset_slug: qm7b
main_figure: /figures/2502.12638/main_figure.jpegoptim.jpg
---

