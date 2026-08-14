---
title: PCQM4Mv2
slug: pcqm4mv2
benchmark: OGB
task_type: graph_regression
short_description: Predict each molecule's HOMO-LUMO energy gap, a continuous quantum-chemical
  property calculated with density functional theory.
description: '**Graph regression** Predict each molecule''s HOMO-LUMO energy gap,
  a continuous quantum-chemical property calculated with density functional theory.
  The default 2D graph conversion uses OGB''s nine categorical atom and three categorical
  bond fields from SMILES. Evaluated by MAE.'
detailed_description:
  task: Predict each molecule's HOMO-LUMO energy gap, a continuous quantum-chemical
    property calculated with density functional theory. Mean absolute error in electron
    volts is the official metric.
  data: PCQM4Mv2 contains 3,746,619 PubChemQC molecules. Training molecules also have
    DFT-optimized 3D structures, while SMILES describe the final optimized connectivity;
    test labels are held by OGB-LSC.
  features: The default 2D graph conversion uses OGB's nine categorical atom and three
    categorical bond fields from SMILES. Coordinates are optional additional inputs
    for training molecules and are unavailable in the same form for blind test molecules.
  splits_and_evaluation: Molecules are ordered and split by PubChem compound identifier
    into 90% train, 2% validation, 4% test-dev, and 4% test-challenge. Despite an
    original intention to use scaffolds, the released split is CID-based because of
    a preprocessing bug.
  quirks_and_pitfalls: PCQM4Mv2 corrected an approximately 10% mismatch in PCQM4M
    between initial SMILES and gaps computed after geometry optimization, so the versions
    are not interchangeable. The CID split is not a scaffold split. Test-dev and test-challenge
    are distinct blind sets, and using supplied training coordinates creates an input-availability
    asymmetry.
sources:
- title: OGB-LSC
  arxiv_id: '2103.09430'
  kind: benchmark_definition
- title: Official PCQM4Mv2 documentation
  url: https://ogb.stanford.edu/docs/lsc/pcqm4mv2/
  kind: official_documentation
- title: PubChemQC project
  url: https://doi.org/10.1021/acs.jcim.7b00083
  kind: upstream_data_source
primary_metric: MAE
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.PCQM4Mv2.html
stats:
  num_graphs: 3746619
  avg_nodes: 14.14
  avg_edges: 14.56
  num_classes: null
  extra_stats:
    avg_degree: 2.05
    clustering_coefficient: 0.011
    degree_convention: reported in OGB-LSC Table 8 after standardizing graphs to undirected
      unlabeled graphs
    diameter: 7.95
    edge_feature_dim: 3
    edge_feature_type: categorical bond features from RDKit
    label_imbalance: not applicable; the target is continuous HOMO-LUMO gap regression
    node_feature_dim: 9
    node_feature_type: categorical atom features from RDKit
    statistic_notes: OGB-LSC Table 8 reports average degree, clustering coefficient,
      and diameter on standardized graphs; training molecules additionally have 3D
      coordinates
    target_unit: eV
result_count: 112
best_model:
  model: DeMol
  value: 0.0603
  metric: MAE
  arxiv_id: '2603.00568'
  paper_title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
    and Interactions
papers:
- arxiv_id: '2603.00568'
  title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
    and Interactions
  date_iso: '2026-02-28'
  venue: ICLR 2026
- arxiv_id: '2602.17071'
  title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
    and Self-Corrective Propagation'
  date_iso: '2026-02-19'
  venue: ''
- arxiv_id: '2512.12489'
  title: 'GoMS: Graph of Molecule Substructure Network for Molecule Property Prediction'
  date_iso: '2025-12-13'
  venue: ''
- arxiv_id: '2510.05583'
  title: 'When does global attention help: a unified empirical study on atomistic
    graph learning'
  date_iso: '2025-10-07'
  venue: ''
- arxiv_id: '2402.04538'
  title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
    Learning with Triplet Graph Transformers'
  date_iso: '2024-02-07'
  venue: ICML 2024
- arxiv_id: '2401.10119'
  title: Towards Principled Graph Transformers
  date_iso: '2024-01-18'
  venue: NeurIPS 2024
- arxiv_id: '2312.04234'
  title: Graph Convolutions Enrich the Self-Attention in Transformers!
  date_iso: '2023-12-07'
  venue: NeurIPS 2023
- arxiv_id: '2310.20519'
  title: Enhancing Graph Neural Networks with Quantum Computed Encodings
  date_iso: '2023-10-31'
  venue: ''
- arxiv_id: '2305.11424'
  title: IJCAI--23 Formatting Instructions
  date_iso: '2023-05-19'
  venue: IJCAI 2023
- arxiv_id: '2303.01028'
  title: 'Specformer: Spectral Graph Neural Networks Meet Transformers'
  date_iso: '2023-03-02'
  venue: ICLR 2023
- arxiv_id: '2210.01765'
  title: One Transformer Can Understand Both 2D & 3D Molecular Data
  date_iso: '2022-10-04'
  venue: ICLR 2022
- arxiv_id: '2208.05863'
  title: 'GEM-2: Next Generation Molecular Property Prediction Network by Modeling
    Full-range Many-body Interactions'
  date_iso: '2022-08-11'
  venue: ''
- arxiv_id: '2207.02505'
  title: Pure Transformers are Powerful Graph Learners
  date_iso: '2022-07-06'
  venue: NeurIPS 2022
- arxiv_id: '2205.12454'
  title: Recipe for a General, Powerful, Scalable Graph Transformer
  date_iso: '2022-05-25'
  venue: NeurIPS 2022
- arxiv_id: '2201.12787'
  title: 'GRPE: Relative Positional Encoding for Graph Transformer'
  date_iso: '2022-01-30'
  venue: ''
- arxiv_id: '2107.09422'
  title: Large-scale graph representation learning with very deep GNNs and self-supervision
  date_iso: '2021-07-20'
  venue: KDD 2021
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MAE
  default_metric: MAE
  higher_is_better: false
  stats:
    num_graphs: 3746619
    avg_nodes: 14.14
    avg_edges: 14.56
    num_classes: null
    extra_stats:
      avg_degree: 2.05
      clustering_coefficient: 0.011
      degree_convention: reported in OGB-LSC Table 8 after standardizing graphs to
        undirected unlabeled graphs
      diameter: 7.95
      edge_feature_dim: 3
      edge_feature_type: categorical bond features from RDKit
      label_imbalance: not applicable; the target is continuous HOMO-LUMO gap regression
      node_feature_dim: 9
      node_feature_type: categorical atom features from RDKit
      statistic_notes: OGB-LSC Table 8 reports average degree, clustering coefficient,
        and diameter on standardized graphs; training molecules additionally have
        3D coordinates
      target_unit: eV
  metrics:
  - MAE
  metric_display_names:
  - HOMO-LUMO gap MAE (eV)
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: DeMol
    model_plain: DeMol
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 186.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.0603
    metric_stds:
    - null
  - model: TGT-At
    model_plain: TGT-At
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 203.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0671
    metric_stds:
    - null
  - model: TGT-At (+RDKit)
    model_plain: TGT-At (+RDKit)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 203.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_iso: '2024-02-07'
    date_display: Feb 2024
    codebase_url: https://github.com/shamim-hussain/tgt
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0683
    metric_stds:
    - null
  - model: UniMol
    model_plain: UniMol
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 77.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0693
    metric_stds:
    - null
  - model: Uni-Mol+ (+RDKit)
    model_plain: Uni-Mol+ (+RDKit)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 77.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_iso: '2024-02-07'
    date_display: Feb 2024
    codebase_url: https://github.com/shamim-hussain/tgt
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0705
    metric_stds:
    - null
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 44.3
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_iso: '2024-02-07'
    date_display: Feb 2024
    codebase_url: https://github.com/shamim-hussain/tgt
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.072
    metric_stds:
    - null
  - model: Transformer-M
    model_plain: Transformer-M
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 69.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0772
    metric_stds:
    - null
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 44.3
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0778
    metric_stds:
    - null
  - model: GoMS_GT
    model_plain: GoMS_GT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2512.12489'
    title: 'GoMS: Graph of Molecule Substructure Network for Molecule Property Prediction'
    date: Dec 13, 2025
    date_iso: '2025-12-13'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.078
    metric_stds:
    - null
  - model: Transformer-M
    model_plain: Transformer-M
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 69.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_iso: '2024-02-07'
    date_display: Feb 2024
    codebase_url: https://github.com/shamim-hussain/tgt
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0782
    metric_stds:
    - null
  - model: Transformer-M
    model_plain: Transformer-M
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2210.01765'
    title: One Transformer Can Understand Both 2D & 3D Molecular Data
    date: Oct 4, 2022
    date_iso: '2022-10-04'
    date_display: Oct 2022
    codebase_url: https://github.com/lsj2408/Transformer-M
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0787
    metric_stds:
    - null
  - model: GEM-2
    model_plain: GEM-2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 32.1
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0793
    metric_stds:
    - null
  - model: MPNNs
    model_plain: MPNNs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12489'
    title: 'GoMS: Graph of Molecule Substructure Network for Molecule Property Prediction'
    date: Dec 13, 2025
    date_iso: '2025-12-13'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.08
    metric_stds:
    - null
  - model: GEM-2 (+RDKit)
    model_plain: GEM-2 (+RDKit)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 32.1
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_iso: '2024-02-07'
    date_display: Feb 2024
    codebase_url: https://github.com/shamim-hussain/tgt
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.08059999999999999
    metric_stds:
    - null
  - model: GEM-2
    model_plain: GEM-2
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 32.1
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2208.05863'
    title: 'GEM-2: Next Generation Molecular Property Prediction Network by Modeling
      Full-range Many-body Interactions'
    date: Aug 11, 2022
    date_iso: '2022-08-11'
    date_display: Aug 2022
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0806
    metric_stds:
    - null
  - model: GPTrans-L
    model_plain: GPTrans-L
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0809
    metric_stds:
    - null
  - model: GPTrans-B
    model_plain: GPTrans-B
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0813
    metric_stds:
    - null
  - model: GPTrans-S
    model_plain: GPTrans-S
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0823
    metric_stds:
    - null
  - model: ET+RRWP
    model_plain: ET+RRWP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2401.10119'
    title: Towards Principled Graph Transformers
    date: Jan 18, 2024
    date_iso: '2024-01-18'
    date_display: Jan 2024
    codebase_url: https://github.com/luis-mueller/towards-principled-gts
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0832
    metric_stds:
    - null
  - model: GPTrans-T
    model_plain: GPTrans-T
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0833
    metric_stds:
    - null
  - model: GRIT 2-QiQRW
    model_plain: GRIT 2-QiQRW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0838
    metric_stds:
    - null
  - model: ET
    model_plain: ET
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.10119'
    title: Towards Principled Graph Transformers
    date: Jan 18, 2024
    date_iso: '2024-01-18'
    date_display: Jan 2024
    codebase_url: https://github.com/luis-mueller/towards-principled-gts
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.084
    metric_stds:
    - null
  - model: GRIT (our run)
    model_plain: GRIT (our run)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0842
    metric_stds:
    - null
  - model: GPS-Deep
    model_plain: GPS-Deep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 138.1
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0852
    metric_stds:
    - null
  - model: GraphGPS_DEEP
    model_plain: GraphGPS_DEEP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 13.8
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0852
    metric_stds:
    - null
  - model: GraphGPS Medium
    model_plain: GraphGPS Medium
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.4
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.10119'
    title: Towards Principled Graph Transformers
    date: Jan 18, 2024
    date_iso: '2024-01-18'
    date_display: Jan 2024
    codebase_url: https://github.com/luis-mueller/towards-principled-gts
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0858
    metric_stds:
    - null
  - model: GTs
    model_plain: GTs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0858
    metric_stds:
    - null
  - model: GPS-medium
    model_plain: GPS-medium
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.4
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2303.01028'
    title: 'Specformer: Spectral Graph Neural Networks Meet Transformers'
    date: Mar 2, 2023
    date_iso: '2023-03-02'
    date_display: Mar 2023
    codebase_url: https://github.com/bdy9527/Specformer
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0858
    metric_stds:
    - null
  - model: GraphGPS_BASE
    model_plain: GraphGPS_BASE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.4
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.01765'
    title: One Transformer Can Understand Both 2D & 3D Molecular Data
    date: Oct 4, 2022
    date_iso: '2022-10-04'
    date_display: Oct 2022
    codebase_url: https://github.com/lsj2408/Transformer-M
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0858
    metric_stds:
    - null
  - model: EGT-Larger
    model_plain: EGT-Larger
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 110.8
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0859
    metric_stds:
    - null
  - model: GRIT
    model_plain: GRIT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.6
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.10119'
    title: Towards Principled Graph Transformers
    date: Jan 18, 2024
    date_iso: '2024-01-18'
    date_display: Jan 2024
    codebase_url: https://github.com/luis-mueller/towards-principled-gts
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0859
    metric_stds:
    - null
  - model: OSAN
    model_plain: OSAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12489'
    title: 'GoMS: Graph of Molecule Substructure Network for Molecule Property Prediction'
    date: Dec 13, 2025
    date_iso: '2025-12-13'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0862
    metric_stds:
    - null
  - model: EGT
    model_plain: EGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 89.3
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2208.05863'
    title: 'GEM-2: Next Generation Molecular Property Prediction Network by Modeling
      Full-range Many-body Interactions'
    date: Aug 11, 2022
    date_iso: '2022-08-11'
    date_display: Aug 2022
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0862
    metric_stds:
    - null
  - model: GraphGPS
    model_plain: GraphGPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 13.8
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_iso: '2024-02-07'
    date_display: Feb 2024
    codebase_url: https://github.com/shamim-hussain/tgt
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0862
    metric_stds:
    - null
  - model: Graphormer
    model_plain: Graphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0864
    metric_stds:
    - null
  - model: GRPE-Large
    model_plain: GRPE-Large
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 118.3
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0867
    metric_stds:
    - null
  - model: GRPE_LARGE
    model_plain: GRPE_LARGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2210.01765'
    title: One Transformer Can Understand Both 2D & 3D Molecular Data
    date: Oct 4, 2022
    date_iso: '2022-10-04'
    date_display: Oct 2022
    codebase_url: https://github.com/lsj2408/Transformer-M
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0867
    metric_stds:
    - null
  - model: EGT-Large
    model_plain: EGT-Large
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 89.3
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0869
    metric_stds:
    - null
  - model: EGT
    model_plain: EGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0869
    metric_stds:
    - null
  - model: Graphormer
    model_plain: Graphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2512.12489'
    title: 'GoMS: Graph of Molecule Substructure Network for Molecule Property Prediction'
    date: Dec 13, 2025
    date_iso: '2025-12-13'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.087
    metric_stds:
    - null
  - model: EGT-Large
    model_plain: EGT-Large
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 110.8
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_iso: '2022-01-30'
    date_display: Jan 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0872
    metric_stds:
    - null
  - model: GRPE-Large
    model_plain: GRPE-Large
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 118.3
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2208.05863'
    title: 'GEM-2: Next Generation Molecular Property Prediction Network by Modeling
      Full-range Many-body Interactions'
    date: Aug 11, 2022
    date_iso: '2022-08-11'
    date_display: Aug 2022
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0876
    metric_stds:
    - null
  - model: GRPE
    model_plain: GRPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 118.3
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_iso: '2024-02-07'
    date_display: Feb 2024
    codebase_url: https://github.com/shamim-hussain/tgt
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0876
    metric_stds:
    - null
  - model: EGT-Medium
    model_plain: EGT-Medium
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 47.4
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0881
    metric_stds:
    - null
  - model: IDMPNN
    model_plain: IDMPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12489'
    title: 'GoMS: Graph of Molecule Substructure Network for Molecule Property Prediction'
    date: Dec 13, 2025
    date_iso: '2025-12-13'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0882
    metric_stds:
    - null
  - model: GraphormerV2-L
    model_plain: GraphormerV2-L
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 159.3
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0883
    metric_stds:
    - null
  - model: GRPE-Standard
    model_plain: GRPE-Standard
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.089
    metric_stds:
    - null
  - model: GRPE
    model_plain: GRPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.089
    metric_stds:
    - null
  - model: GRPE_BASE
    model_plain: GRPE_BASE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2210.01765'
    title: One Transformer Can Understand Both 2D & 3D Molecular Data
    date: Oct 4, 2022
    date_iso: '2022-10-04'
    date_display: Oct 2022
    codebase_url: https://github.com/lsj2408/Transformer-M
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.089
    metric_stds:
    - null
  - model: GRPE-Standard
    model_plain: GRPE-Standard
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_iso: '2022-01-30'
    date_display: Jan 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0898
    metric_stds:
    - null
  row_count: 112
  rows_json: /data/datasets/pcqm4mv2/standard-split-rows.json
  chart_json: /data/datasets/pcqm4mv2/standard-split-chart.json
  arch_counts:
    gnn: 41
    hybrid: 24
    graph_transformer: 41
    llm: 0
    walk: 0
    traditional: 2
  metric_counts:
  - 112
  milestones: &id001
  - value: 0.1205
    std: null
    model: ILSVRC
    arxiv_id: '2107.09422'
    title: Large-scale graph representation learning with very deep GNNs and self-supervision
    date: '2021-07-20'
  - value: 0.0872
    std: null
    model: EGT-Large
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: '2022-01-30'
  - value: 0.0858
    std: null
    model: GTs
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: '2022-05-25'
  - value: 0.0806
    std: null
    model: GEM-2
    arxiv_id: '2208.05863'
    title: 'GEM-2: Next Generation Molecular Property Prediction Network by Modeling
      Full-range Many-body Interactions'
    date: '2022-08-11'
  - value: 0.0787
    std: null
    model: Transformer-M
    arxiv_id: '2210.01765'
    title: One Transformer Can Understand Both 2D & 3D Molecular Data
    date: '2022-10-04'
  - value: 0.0683
    std: null
    model: TGT-At (+RDKit)
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: '2024-02-07'
  - value: 0.0603
    std: null
    model: DeMol
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: '2026-02-28'
  milestones_by_metric:
    MAE: *id001
---

