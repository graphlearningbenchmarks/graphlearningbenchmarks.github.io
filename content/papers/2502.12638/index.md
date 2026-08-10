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
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 2
  total: 9
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ESOL
  rows:
  - model: Graphormer-SPIS
    model_key: graphormer-spis
    model_plain: Graphormer-SPIS
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
    global_rank: 1
    sort_value: 0.484
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPD
    model_key: graphormer-spd
    model_plain: Graphormer-SPD
    value: 0.492
    std: 0.004
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
    global_rank: 2
    sort_value: 0.492
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: conan-FGW
    model_key: conan-fgw
    model_plain: conan-FGW
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
    global_rank: 7
    paper_rank: 127
    rank_delta: 120
    rank_delta_abs: 120
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Structural Expressive Power of Graph Transformers
    comparison_source_arxiv: '2305.13987'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.601
    std: 0.008
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 18
    sort_value: 0.601
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
    global_rank: 25
    paper_rank: 127
    rank_delta: 102
    rank_delta_abs: 102
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
    global_rank: 27
    paper_rank: 81
    rank_delta: 54
    rank_delta_abs: 54
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
    global_rank: 64
    paper_rank: 64
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
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
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
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.05599999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: 0.028
    global_rank: 65
    paper_rank: 77
    rank_delta: 12
    rank_delta_abs: 12
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
    value_gap_source_date_iso: '2026-04-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.918
    true_std: null
    value_gap_source_arxiv: '2604.06336'
    value_gap_source_title: 'BiScale-GTR: Fragment-Aware Graph Transformers for Multi-Scale
      Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.15200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.918
    sort_std: null
    global_rank: 70
    paper_rank: 93
    rank_delta: 23
    rank_delta_abs: 23
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
    global_rank: 90
    paper_rank: 91
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
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
    true_value: 1.11
    true_std: 0.01
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.11
    sort_std: 0.01
    global_rank: 103
    paper_rank: 103
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
    global_rank: 118
    paper_rank: 118
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
    global_rank: 121
    paper_rank: 121
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
    global_rank: 127
    paper_rank: 127
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
    global_rank: 130
    paper_rank: 130
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
  - model: SE(3)-I MPPH
    model_key: se(3)-i mpph
    model_plain: SE(3)-I MPPH
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
  - model: ECFP-4 + RF
    model_key: ecfp-4 + rf
    model_plain: ECFP-4 + RF
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
  - model: GPSE + GPS
    model_key: gpse + gps
    model_plain: GPSE + GPS
    value: 0.682
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.07107'
    title: Graph Positional and Structural Encoder
    date: Jul 14, 2023
    date_display: Jul 2023
    date_iso: '2023-07-14'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/G-Taxonomy-Workgroup/GPSE
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.682
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
    global_rank: 12
    paper_rank: 58
    rank_delta: 46
    rank_delta_abs: 46
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
    global_rank: 30
    paper_rank: 30
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
    global_rank: 36
    paper_rank: 36
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
    global_rank: 50
    paper_rank: 50
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
    global_rank: 51
    paper_rank: 51
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
    true_value: 2.2
    true_std: 0.2
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.2
    sort_std: 0.2
    global_rank: 62
    paper_rank: 62
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
    global_rank: 63
    paper_rank: 63
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
    global_rank: 69
    paper_rank: 84
    rank_delta: 15
    rank_delta_abs: 15
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
    global_rank: 77
    paper_rank: 90
    rank_delta: 13
    rank_delta_abs: 13
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
    global_rank: 99
    paper_rank: 99
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
    global_rank: 100
    paper_rank: 100
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
    global_rank: 103
    paper_rank: 103
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
    global_rank: 106
    paper_rank: 106
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
results_grouped:
- benchmark: MoleculeNet
  datasets:
  - *id001
  - *id002
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
main_figure: /figures/2502.12638/main_figure.jpegoptim.jpg
---

