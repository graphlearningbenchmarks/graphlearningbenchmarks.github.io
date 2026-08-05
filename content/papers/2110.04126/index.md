---
title: 3D Infomax improves GNNs for Molecular Property Prediction
arxiv_id: '2110.04126'
source_url: ''
authors:
- name: Hannes Stärk
  orcid: null
  s2_author_id: '2124211700'
  s2_url: null
- name: D. Beaini
  orcid: null
  s2_author_id: '51034451'
  s2_url: null
- name: Gabriele Corso
  orcid: null
  s2_author_id: '1630330616'
  s2_url: null
- name: Prudencio Tossou
  orcid: null
  s2_author_id: '12611623'
  s2_url: null
- name: Christian Dallago
  orcid: null
  s2_author_id: '35805107'
  s2_url: null
- name: Stephan Gunnemann
  orcid: null
  s2_author_id: '51249380'
  s2_url: null
- name: Pietro Liò
  orcid: null
  s2_author_id: '2284767068'
  s2_url: null
published_date: Oct 8, 2021
published_date_iso: '2021-10-08'
published_venue: ICML 2021
published_conference: ICML 2021
published_conference_short: ICML
published_conference_slug: icml
abstract: Molecular property prediction is one of the fastest-growing applications
  of deep learning with critical real-world impacts. Including 3D molecular structure
  as input to learned models improves their performance for many molecular tasks.
  However, this information is infeasible to compute at the scale required by several
  real-world applications. We propose pre-training a model to reason about the geometry
  of molecules given only their 2D molecular graphs. Using methods from self-supervised
  learning, we maximize the mutual information between 3D summary vectors and the
  representations of a Graph Neural Network (GNN) such that they contain latent 3D
  information. During fine-tuning on molecules with unknown geometry, the GNN still
  generates implicit 3D information and can use it to improve downstream tasks. We
  show that 3D pre-training provides significant improvements for a wide range of
  properties, such as a 22% average MAE reduction on eight quantum mechanical properties.
  Moreover, the learned representations can be effectively transferred between datasets
  in different molecular spaces.
codebase_url: https://github.com/HannesStark/3DInfomax
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- 3D Infomax
- 3D Infomax QM9
- 3D Infomax Drugs
- 3D Infomax QMugs
mrr: 0.0145
adjusted_mrr: 0.0097
mrr_dataset_count: 2
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
  - model: 10% ZINC + 10% PubChem
    model_key: 10% zinc + 10% pubchem
    model_plain: 10% ZINC + 10% PubChem
    value: 0.2775
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.2775
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MAT
    model_key: mat
    model_plain: MAT
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
    global_rank: 2
    sort_value: 0.278
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MoLFormer-XL
    model_key: molformer-xl
    model_plain: MoLFormer-XL
    value: 0.2787
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.2787
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.564
    std: 0.015
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
    global_rank: 13
    sort_value: 0.564
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ConfGen
    model_key: confgen
    model_plain: ConfGen
    value: 0.867
    std: 0.045
    paper_value: 0.867
    paper_std: 0.045
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for esol
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.867
    true_std: 0.045
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.867
    sort_std: 0.045
    global_rank: 69
    paper_rank: 69
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
    value: 0.894
    std: 0.028
    paper_value: 0.894
    paper_std: 0.028
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for esol
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.894
    true_std: 0.028
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: 0.028
    global_rank: 71
    paper_rank: 71
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Rand Init
    model_key: rand init
    model_plain: Rand Init
    value: 0.947
    std: 0.038
    paper_value: 0.947
    paper_std: 0.038
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for esol
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.947
    true_std: 0.038
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.947
    sort_std: 0.038
    global_rank: 83
    paper_rank: 83
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
    value: 0.959
    std: 0.047
    paper_value: 0.959
    paper_std: 0.047
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for esol
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.959
    true_std: 0.047
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.959
    sort_std: 0.047
    global_rank: 85
    paper_rank: 85
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DisPred
    model_key: dispred
    model_plain: DisPred
    value: 0.986
    std: 0.025
    paper_value: 0.986
    paper_std: 0.025
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for esol
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.986
    true_std: 0.025
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.986
    sort_std: 0.025
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
  - model: 10% ZINC + 10% PubChem
    model_key: 10% zinc + 10% pubchem
    model_plain: 10% ZINC + 10% PubChem
    value: 0.205
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.205
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MoLFormer-XL
    model_key: molformer-xl
    model_plain: MoLFormer-XL
    value: 0.2308
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.2308
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoLFormer-Base
    model_key: molformer-base
    model_plain: MoLFormer-Base
    value: 0.2596
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.2596
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3D Infomax
    model_key: 3d infomax
    model_plain: 3D Infomax
    value: 2.337
    std: 0.227
    paper_value: 2.337
    paper_std: 0.227
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for freesolv
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
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
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 2.23
    true_std: 0.26
    value_gap_source_arxiv: '2502.12638'
    value_gap_source_title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for
      3D Molecule Generation'
    value_gap_source_is_current_paper: false
    value_gap: 0.1070000000000002
    has_value_note: false
    value_note: ''
    sort_value: 2.23
    sort_std: 0.26
    global_rank: 67
    paper_rank: 71
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Rand Init
    model_key: rand init
    model_plain: Rand Init
    value: 2.233
    std: 0.261
    paper_value: 2.233
    paper_std: 0.261
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for freesolv
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.233
    true_std: 0.261
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.233
    sort_std: 0.261
    global_rank: 68
    paper_rank: 68
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
    value: 2.346
    std: 0.122
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_display: Jun 2021
    date_iso: '2021-06-11'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 73
    sort_value: 2.346
    sort_std: 0.122
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ConfGen
    model_key: confgen
    model_plain: ConfGen
    value: 2.428
    std: 0.155
    paper_value: 2.428
    paper_std: 0.155
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for freesolv
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.428
    true_std: 0.155
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.428
    sort_std: 0.155
    global_rank: 75
    paper_rank: 75
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DisPred
    model_key: dispred
    model_plain: DisPred
    value: 2.486
    std: 0.222
    paper_value: 2.486
    paper_std: 0.222
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for freesolv
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.486
    true_std: 0.222
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.486
    sort_std: 0.222
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 3.744
    std: 0.292
    paper_value: 3.744
    paper_std: 0.292
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard RMSE for freesolv
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 3.166
    true_std: 0.027
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.5780000000000003
    has_value_note: false
    value_note: ''
    sort_value: 3.166
    sort_std: 0.027
    global_rank: 105
    paper_rank: 115
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
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
  dataset: QM9
  is_multi_metric: true
  rows:
  - model: PF-GNN
    model_key: pf-gnn
    model_plain: PF-GNN
    metric_values:
    - 0.017
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    published_venue: ''
    date: Jan 31, 2024
    date_display: Jan 2024
    date_iso: '2024-01-31'
    codebase_url: https://github.com/pfgnn/PF-GNN
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.017
    sort_std: 0.001
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    metric_values:
    - 0.019
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    published_venue: ''
    date: Jan 31, 2024
    date_display: Jan 2024
    date_iso: '2024-01-31'
    codebase_url: https://github.com/pfgnn/PF-GNN
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.019
    sort_std: 0.001
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: Molformer
    model_key: molformer
    model_plain: Molformer
    metric_values:
    - 0.025
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    published_venue: ''
    date: Oct 4, 2021
    date_display: Oct 2021
    date_iso: '2021-10-04'
    codebase_url: https://github.com/smiles724/Molformer
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.025
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: 3D Infomax
    model_key: 3d infomax
    model_plain: 3D Infomax
    metric_values:
    - null
    - 68.96
    - 69.51
    - 7.966
    - 17.39
    - null
    - null
    - 0.1306
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 68.96
    sort_std: null
    true_value: 68.96
    true_std: null
    paper_value: 68.96
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 44
  - model: True 3D SMP
    model_key: true 3d smp
    model_plain: True 3D SMP
    metric_values:
    - 85.1
    - null
    - null
    - null
    - null
    - 0.0726
    - 0.1542
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 85.1
    sort_std: null
    true_value: 85.1
    true_std: null
    paper_value: 85.1
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 39
  - model: 3D Infomax QM9
    model_key: 3d infomax qm9
    model_plain: 3D Infomax QM9
    metric_values:
    - 101.71
    - null
    - null
    - null
    - null
    - 0.3507
    - 0.3268
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 101.71
    sort_std: null
    true_value: 101.71
    true_std: null
    paper_value: 101.71
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 46
  - model: 3D Infomax Drugs
    model_key: 3d infomax drugs
    model_plain: 3D Infomax Drugs
    metric_values:
    - 102.59
    - null
    - null
    - null
    - null
    - 0.3512
    - 0.2959
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 102.59
    sort_std: null
    true_value: 102.59
    true_std: null
    paper_value: 102.59
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 48
  - model: 3D Infomax QMugs
    model_key: 3d infomax qmugs
    model_plain: 3D Infomax QMugs
    metric_values:
    - 103.85
    - null
    - null
    - null
    - null
    - 0.3668
    - 0.2807
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 103.85
    sort_std: null
    true_value: 103.85
    true_std: null
    paper_value: 103.85
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 49
  - model: ConfGen
    model_key: confgen
    model_plain: ConfGen
    metric_values:
    - 110.72
    - null
    - null
    - null
    - null
    - 0.394
    - 0.4219
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 110.72
    sort_std: null
    true_value: 110.72
    true_std: null
    paper_value: 110.72
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 51
  - model: RDKit
    model_key: rdkit
    model_plain: RDKit
    metric_values:
    - 114.24
    - null
    - null
    - null
    - null
    - 0.4344
    - 0.302
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 114.24
    sort_std: null
    true_value: 114.24
    true_std: null
    paper_value: 114.24
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 52
  - model: DisPred
    model_key: dispred
    model_plain: DisPred
    metric_values:
    - 116.21
    - null
    - null
    - null
    - null
    - 0.4626
    - 0.357
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 116.21
    sort_std: null
    true_value: 116.21
    true_std: null
    paper_value: 116.21
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 53
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    metric_values:
    - 120.08
    - null
    - null
    - null
    - null
    - 0.3937
    - 0.3295
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 120.08
    sort_std: null
    true_value: 120.08
    true_std: null
    paper_value: 120.08
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 54
  - model: Rand Init
    model_key: rand init
    model_plain: Rand Init
    metric_values:
    - 123.08
    - null
    - null
    - null
    - null
    - 0.4133
    - 0.3972
    - null
    metric_stds:
    - 3.98
    - null
    - null
    - null
    - null
    - 0.003
    - 0.014
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 123.08
    sort_std: 3.98
    true_value: 123.08
    true_std: 3.98
    paper_value: 123.08
    paper_std: 3.98
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
    global_rank: 55
  - model: ProPred
    model_key: propred
    model_plain: ProPred
    metric_values:
    - 131.99
    - null
    - null
    - null
    - null
    - 0.3975
    - 0.3732
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 131.99
    sort_std: null
    true_value: 131.99
    true_std: null
    paper_value: 131.99
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICML 2021
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 56
  metrics:
  - gap
  - HOMO
  - LUMO
  - zpve
  - R2
  - mu
  - alpha
  - Cv
  primary_metric: gap
  rank_metric: gap
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: gap
  paper_metrics:
  - HOMO
  - LUMO
  - zpve
  - R2
  - mu
  - alpha
  - gap
  - Cv
  metric: gap
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
    - dataset: QM9
      dataset_slug: qm9
main_figure: /figures/2110.04126/main_figure.jpegoptim.jpg
---

