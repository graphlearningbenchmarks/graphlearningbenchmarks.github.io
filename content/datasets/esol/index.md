---
title: ESOL
slug: esol
benchmark: MoleculeNet
task_type: graph_regression
short_description: Aqueous solubility regression (log mol/L) on 1,128 molecules.
description: '**Graph regression** Aqueous solubility regression (log mol/L) on 1,128
  molecules. SMILES and labels are fixed; molecular graph featurization is implementation-defined.
  Random and scaffold splits are not comparable. Evaluated by RMSE.'
detailed_description:
  task: Aqueous solubility regression (log mol/L) on 1,128 molecules. The primary
    catalog metric is RMSE.
  data: Aqueous solubility regression (log mol/L) on 1,128 molecules.
  features: MoleculeNet distributes SMILES and targets, not one mandatory graph featurization.
    A graph implementation normally derives atom and bond fields with RDKit or DeepChem;
    results depend on featurizer, salt handling, stereochemistry, and invalid-molecule
    policy.
  splits_and_evaluation: 'The catalog records these protocols or variants: Scaffold
    split. Evaluation uses RMSE (lower is better). Exact masks or folds must come
    from the cited release.'
  quirks_and_pitfalls: Small samples, imbalance, missing assay labels, duplicate compounds,
    and scaffold leakage are common. Missing labels are not negatives. Always report
    split algorithm, featurizer, metric aggregation, and dataset version; random and
    scaffold results are not comparable.
sources:
- title: MoleculeNet benchmark
  arxiv_id: '1703.00564'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric ESOL loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
  kind: implementation_documentation
primary_metric: RMSE
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
stats: null
result_count: 186
best_model:
  model: Graphormer-SPIS
  value: 0.484
  metric: RMSE
  arxiv_id: '2305.13987'
  paper_title: On Structural Expressive Power of Graph Transformers
papers:
- arxiv_id: '2604.06336'
  title: 'BiScale-GTR: Fragment-Aware Graph Transformers for Multi-Scale Molecular
    Representation Learning'
  date_iso: '2026-04-07'
  venue: ''
- arxiv_id: '2602.20344'
  title: Hierarchical Molecular Representation Learning via Fragment-Based Self-Supervised
    Embedding Prediction
  date_iso: '2026-02-23'
  venue: ''
- arxiv_id: '2510.07289'
  title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D Graph Encoder'
  date_iso: '2025-10-08'
  venue: ''
- arxiv_id: '2502.12638'
  title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation'
  date_iso: '2025-02-18'
  venue: ICLR 2025
- arxiv_id: '2412.15589'
  title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
    Graph Information Bottleneck
  date_iso: '2024-12-20'
  venue: AAAI 2024
- arxiv_id: '2405.10343'
  title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view Molecular
    Representation Learning'
  date_iso: '2024-05-15'
  venue: ICML 2024
- arxiv_id: '2402.01975'
  title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
  date_iso: '2024-02-03'
  venue: ICML 2024
- arxiv_id: '2312.07633'
  title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive Molecular
    Property Prediction
  date_iso: '2023-12-12'
  venue: NeurIPS 2023
- arxiv_id: '2310.16401'
  title: Graph Neural Networks with a Distribution of Parametrized Graphs
  date_iso: '2023-10-25'
  venue: ICML 2023
- arxiv_id: '2310.07351'
  title: Atom-Motif Contrastive Transformer for Molecular Property Prediction
  date_iso: '2023-10-11'
  venue: ''
- arxiv_id: '2309.10131'
  title: Deep Prompt Tuning for Graph Transformers
  date_iso: '2023-09-18'
  venue: ''
- arxiv_id: '2309.04062'
  title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising and
    Cross-Modal Distillation'
  date_iso: '2023-09-08'
  venue: AAAI 2023
- arxiv_id: '2309.04589'
  title: Motif-aware Attribute Masking for Molecular Graph Pre-training
  date_iso: '2023-09-08'
  venue: ''
- arxiv_id: '2305.13987'
  title: On Structural Expressive Power of Graph Transformers
  date_iso: '2023-05-23'
  venue: KDD 2023
- arxiv_id: '2305.13315'
  title: 3D Molecular Geometry Analysis with 2D Graphs
  date_iso: '2023-05-01'
  venue: ''
- arxiv_id: '2209.15101'
  title: Improving Molecular Pretraining with Complementary Featurizations
  date_iso: '2022-09-29'
  venue: ''
- arxiv_id: '2202.09346'
  title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation and
    Decomposed Fragment Contrast
  date_iso: '2022-02-18'
  venue: ''
- arxiv_id: '2112.03806'
  title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
  date_iso: '2021-12-07'
  venue: ''
- arxiv_id: '2112.00544'
  title: Molecular Contrastive Learning with Chemical Element Knowledge Graph
  date_iso: '2021-12-01'
  venue: AAAI 2021
- arxiv_id: '2110.04126'
  title: 3D Infomax improves GNNs for Molecular Property Prediction
  date_iso: '2021-10-08'
  venue: ICML 2021
- arxiv_id: '2110.07728'
  title: 16 Pre-training Molecular Graph Representation with 3D Geometry
  date_iso: '2021-10-07'
  venue: ICLR 2021
- arxiv_id: '2109.11730'
  title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
  date_iso: '2021-09-24'
  venue: AAAI 2021
- arxiv_id: '2106.06130'
  title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
    Prediction'
  date_iso: '2021-06-11'
  venue: ''
- arxiv_id: '2006.04804'
  title: Optimal Transport Graph Neural Networks
  date_iso: '2020-06-08'
  venue: ''
- arxiv_id: '2002.09518'
  title: Memory-Based Graph Networks
  date_iso: '2020-02-21'
  venue: ICLR 2020
- arxiv_id: '1703.00564'
  title: MoleculeNet
  date_iso: '2017-03-02'
  venue: ''
variants:
- slug: scaffold-split
  name: Scaffold split
  notes: ''
  is_standard: true
  primary_metric: RMSE
  default_metric: RMSE
  higher_is_better: false
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - RMSE
  metric_display_names:
  - RMSE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: Graphormer-SPIS
    model_plain: Graphormer-SPIS
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
    date_iso: '2023-05-23'
    date_display: May 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.484
    metric_stds:
    - 0.005
  - model: Graphormer-SPD
    model_plain: Graphormer-SPD
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
    date_iso: '2023-05-23'
    date_display: May 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.492
    metric_stds:
    - 0.004
  - model: conan-FGW
    model_plain: conan-FGW
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
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.514
    metric_stds:
    - 0.019
  - model: MemGNN
    model_plain: MemGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_iso: '2020-02-21'
    date_display: Feb 2020
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.54
    metric_stds:
    - 0.01
  - model: GAT
    model_plain: GAT
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
    date_iso: '2023-05-23'
    date_display: May 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.552
    metric_stds:
    - 0.007
  - model: GeomMPNN
    model_plain: GeomMPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.555
    metric_stds:
    - null
  - model: GCN
    model_plain: GCN
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
    date_iso: '2023-05-23'
    date_display: May 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.564
    metric_stds:
    - 0.015
  - model: LiGhT FT
    model_plain: LiGhT FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 90.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.565
    metric_stds:
    - 0.041
  - model: GeomGCL
    model_plain: GeomGCL
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
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.575
    metric_stds:
    - null
  - model: AttentiveFP
    model_plain: AttentiveFP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.578
    metric_stds:
    - null
  - model: LiGhT DeepGPT
    model_plain: LiGhT DeepGPT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.37
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.579
    metric_stds:
    - 0.038
  - model: MoleculeNet
    model_plain: MoleculeNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_iso: '2023-05-23'
    date_display: May 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.58
    metric_stds:
    - null
  - model: MPNN
    model_plain: MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_iso: '2017-03-02'
    date_display: Mar 2017
    codebase_url: https://github.com/deepchem/deepchem
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.58
    metric_stds:
    - 0.03
  - model: KCL
    model_plain: KCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.00544'
    title: Molecular Contrastive Learning with Chemical Element Knowledge Graph
    date: Dec 1, 2021
    date_iso: '2021-12-01'
    date_display: Dec 2021
    codebase_url: https://github.com/ZJU-Fangyin/KCL
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.582
    metric_stds:
    - null
  - model: CoMPT
    model_plain: CoMPT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.589
    metric_stds:
    - null
  - model: conan
    model_plain: conan
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.591
    metric_stds:
    - 0.025
  - model: ProtoW-Dot
    model_plain: ProtoW-Dot
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_iso: '2020-06-08'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.594
    metric_stds:
    - 0.031
  - model: GraphSAGE
    model_plain: GraphSAGE
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
    date_iso: '2023-05-23'
    date_display: May 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.601
    metric_stds:
    - 0.008
  - model: ProtoW-L2
    model_plain: ProtoW-L2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_iso: '2020-06-08'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.605
    metric_stds:
    - 0.029
  - model: Weave
    model_plain: Weave
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_iso: '2017-03-02'
    date_display: Mar 2017
    codebase_url: https://github.com/deepchem/deepchem
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.61
    metric_stds:
    - 0.07
  - model: ProtoS-L2
    model_plain: ProtoS-L2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.065
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_iso: '2020-06-08'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.611
    metric_stds:
    - 0.034
  - model: Graphormer-id
    model_plain: Graphormer-id
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
    date_iso: '2023-05-23'
    date_display: May 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.612
    metric_stds:
    - 0.002
  - model: SE(3)-I MPPH
    model_plain: SE(3)-I MPPH
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
    date_iso: '2023-12-12'
    date_display: Dec 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.612
    metric_stds:
    - 0.083
  - model: MAT
    model_plain: MAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.624
    metric_stds:
    - null
  - model: DimeNet++
    model_plain: DimeNet++
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.633
    metric_stds:
    - null
  - model: SchNet-emb
    model_plain: SchNet-emb
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.635
    metric_stds:
    - 0.057
  - model: D-MPNN
    model_plain: D-MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_iso: '2020-06-08'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.635
    metric_stds:
    - 0.027
  - model: Graphormer-Neighbor
    model_plain: Graphormer-Neighbor
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
    date_iso: '2023-05-23'
    date_display: May 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.639
    metric_stds:
    - 0.034
  - model: DMPNN
    model_plain: DMPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.647
    metric_stds:
    - null
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.671
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_iso: '2020-06-08'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.654
    metric_stds:
    - 0.028
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.626
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_iso: '2020-06-08'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.665
    metric_stds:
    - 0.026
  - model: SchNet-scalar
    model_plain: SchNet-scalar
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.672
    metric_stds:
    - 0.027
  - model: D-MPNN+TopK Pool
    model_plain: D-MPNN+TopK Pool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_iso: '2020-06-08'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.673
    metric_stds:
    - 0.087
  - model: D-MPNN+SAG Pool
    model_plain: D-MPNN+SAG Pool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_iso: '2020-06-08'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.674
    metric_stds:
    - 0.034
  - model: ChemProp3D
    model_plain: ChemProp3D
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.681
    metric_stds:
    - 0.023
  - model: GraphGPS DeepGPT
    model_plain: GraphGPS DeepGPT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.05
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.685
    metric_stds:
    - 0.13
  - model: HMGNN
    model_plain: HMGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.701
    metric_stds:
    - null
  - model: UniMol
    model_plain: UniMol
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2604.06336'
    title: 'BiScale-GTR: Fragment-Aware Graph Transformers for Multi-Scale Molecular
      Representation Learning'
    date: Apr 7, 2026
    date_iso: '2026-04-07'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.707
    metric_stds:
    - null
  - model: MoLlama
    model_plain: MoLlama
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2502.12638'
    title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation'
    date: Feb 18, 2025
    date_iso: '2025-02-18'
    date_display: Feb 2025
    codebase_url: https://github.com/acharkq/NExT-Mol
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.74
    metric_stds:
    - 0.01
  - model: FPGNN
    model_plain: FPGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.06336'
    title: 'BiScale-GTR: Fragment-Aware Graph Transformers for Multi-Scale Molecular
      Representation Learning'
    date: Apr 7, 2026
    date_iso: '2026-04-07'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.747
    metric_stds:
    - null
  - model: MPG
    model_plain: MPG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.06336'
    title: 'BiScale-GTR: Fragment-Aware Graph Transformers for Multi-Scale Molecular
      Representation Learning'
    date: Apr 7, 2026
    date_iso: '2026-04-07'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.758
    metric_stds:
    - null
  - model: GraphGPS FT
    model_plain: GraphGPS FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 14.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.772
    metric_stds:
    - 0.102
  - model: KANO
    model_plain: KANO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.06336'
    title: 'BiScale-GTR: Fragment-Aware Graph Transformers for Multi-Scale Molecular
      Representation Learning'
    date: Apr 7, 2026
    date_iso: '2026-04-07'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.772
    metric_stds:
    - null
  - model: MolPROP
    model_plain: MolPROP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2502.12638'
    title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation'
    date: Feb 18, 2025
    date_iso: '2025-02-18'
    date_display: Feb 2025
    codebase_url: https://github.com/acharkq/NExT-Mol
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.777
    metric_stds:
    - 0.02
  - model: UniMol
    model_plain: UniMol
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.788
    metric_stds:
    - 0.029
  - model: ChemRL-GEM
    model_plain: ChemRL-GEM
    is_baseline: false
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
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.798
    metric_stds:
    - 0.029
  - model: Geometry+Graph
    model_plain: Geometry+Graph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.798
    metric_stds:
    - 0.029
  - model: Graph
    model_plain: Graph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.815
    metric_stds:
    - 0.025
  - model: AMCT
    model_plain: AMCT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.07351'
    title: Atom-Motif Contrastive Transformer for Molecular Property Prediction
    date: Oct 11, 2023
    date_iso: '2023-10-11'
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
    - 0.815
    metric_stds:
    - 0.01
  - model: S-CGIB
    model_plain: S-CGIB
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2412.15589'
    title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
      Graph Information Bottleneck
    date: Dec 20, 2024
    date_iso: '2024-12-20'
    date_display: Dec 2024
    codebase_url: https://github.com/NSLab-CUK/S-CGIB
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.816
    metric_stds:
    - 0.019
  row_count: 186
  rows_json: /data/datasets/esol/scaffold-split-rows.json
  chart_json: /data/datasets/esol/scaffold-split-chart.json
  arch_counts:
    gnn: 113
    hybrid: 36
    graph_transformer: 17
    llm: 3
    walk: 1
    traditional: 13
  metric_counts:
  - 186
  milestones: &id001
  - value: 0.58
    std: 0.03
    model: MPNN
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: '2017-03-02'
  - value: 0.54
    std: 0.01
    model: MemGNN
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: '2020-02-21'
  - value: 0.484
    std: 0.005
    model: Graphormer-SPIS
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: '2023-05-23'
  milestones_by_metric:
    RMSE: *id001
---

