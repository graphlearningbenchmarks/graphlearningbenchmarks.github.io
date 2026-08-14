---
title: Lipophilicity
slug: lipophilicity
benchmark: MoleculeNet
task_type: graph_regression
short_description: Octanol/water distribution coefficient (logD) regression on 4,200
  molecules.
description: '**Graph regression** Octanol/water distribution coefficient (logD) regression
  on 4,200 molecules. SMILES and labels are fixed; molecular graph featurization is
  implementation-defined. Random and scaffold splits are not comparable. Evaluated
  by RMSE.'
detailed_description:
  task: Octanol/water distribution coefficient (logD) regression on 4,200 molecules.
    The primary catalog metric is RMSE.
  data: Octanol/water distribution coefficient (logD) regression on 4,200 molecules.
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
- title: PyTorch Geometric Lipophilicity loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
  kind: implementation_documentation
primary_metric: RMSE
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
stats:
  num_graphs: 4200
  avg_nodes: 27.0
  avg_edges: 29.5
  num_classes: 1
  extra_stats:
    edge_feature_dim: 3
    edge_feature_type: categorical RDKit bond features in the PyG loader
    label_imbalance: not applicable; experimental logD is a continuous regression
      target
    node_feature_dim: 9
    node_feature_type: categorical RDKit atom features in the PyG loader
    statistic_notes: Average edge count is half of the PyG bidirected edge-entry table
result_count: 123
best_model:
  model: MemGNN
  value: 0.556
  metric: RMSE
  arxiv_id: '2002.09518'
  paper_title: Memory-Based Graph Networks
papers:
- arxiv_id: '2602.20344'
  title: Hierarchical Molecular Representation Learning via Fragment-Based Self-Supervised
    Embedding Prediction
  date_iso: '2026-02-23'
  venue: ''
- arxiv_id: '2510.07289'
  title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D Graph Encoder'
  date_iso: '2025-10-08'
  venue: ''
- arxiv_id: '2412.15589'
  title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
    Graph Information Bottleneck
  date_iso: '2024-12-20'
  venue: AAAI 2024
- arxiv_id: '2312.07633'
  title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive Molecular
    Property Prediction
  date_iso: '2023-12-12'
  venue: NeurIPS 2023
- arxiv_id: '2310.16401'
  title: Graph Neural Networks with a Distribution of Parametrized Graphs
  date_iso: '2023-10-25'
  venue: ICML 2023
- arxiv_id: '2309.04589'
  title: Motif-aware Attribute Masking for Molecular Graph Pre-training
  date_iso: '2023-09-08'
  venue: ''
- arxiv_id: '2307.07107'
  title: Graph Positional and Structural Encoder
  date_iso: '2023-07-14'
  venue: ICML 2023
- arxiv_id: '2305.13315'
  title: 3D Molecular Geometry Analysis with 2D Graphs
  date_iso: '2023-05-01'
  venue: ''
- arxiv_id: '2211.03666'
  title: Application of Graph Neural Networks and graph descriptors for graph classification
  date_iso: '2022-11-07'
  venue: ''
- arxiv_id: '2209.15101'
  title: Improving Molecular Pretraining with Complementary Featurizations
  date_iso: '2022-09-29'
  venue: ''
- arxiv_id: '2109.11730'
  title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
  date_iso: '2021-09-24'
  venue: AAAI 2021
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
    num_graphs: 4200
    avg_nodes: 27.0
    avg_edges: 29.5
    num_classes: 1
    extra_stats:
      edge_feature_dim: 3
      edge_feature_type: categorical RDKit bond features in the PyG loader
      label_imbalance: not applicable; experimental logD is a continuous regression
        target
      node_feature_dim: 9
      node_feature_type: categorical RDKit atom features in the PyG loader
      statistic_notes: Average edge count is half of the PyG bidirected edge-entry
        table
  metrics:
  - RMSE
  metric_display_names:
  - RMSE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.556
    metric_stds:
    - 0.023
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.58
    metric_stds:
    - 0.016
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
    - 0.604
    metric_stds:
    - 0.014
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
    - 0.629
    metric_stds:
    - 0.015
  - model: GPS + GPSE
    model_plain: GPS + GPSE
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
    date_iso: '2023-07-14'
    date_display: Jul 2023
    codebase_url: https://github.com/G-Taxonomy-Workgroup/GPSE
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.643
    metric_stds:
    - null
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
    - 0.646
    metric_stds:
    - 0.041
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.655
    metric_stds:
    - 0.036
  - model: GC
    model_plain: GC
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
    - 0.655
    metric_stds:
    - 0.036
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
    - 0.658
    metric_stds:
    - 0.019
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.661
    metric_stds:
    - null
  - model: GPS+LapPE
    model_plain: GPS+LapPE
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
    date_iso: '2023-07-14'
    date_display: Jul 2023
    codebase_url: https://github.com/G-Taxonomy-Workgroup/GPSE
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.662
    metric_stds:
    - null
  - model: GPS + RWSE
    model_plain: GPS + RWSE
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
    date_iso: '2023-07-14'
    date_display: Jul 2023
    codebase_url: https://github.com/G-Taxonomy-Workgroup/GPSE
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.671
    metric_stds:
    - null
  - model: Node-MPN
    model_plain: Node-MPN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.672
    metric_stds:
    - 0.051
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
    - 0.675
    metric_stds:
    - 0.08
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
    - 0.682
    metric_stds:
    - null
  - model: 3D Infomax
    model_plain: 3D Infomax
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.695
    metric_stds:
    - 0.012
  - model: ContextPred
    model_plain: ContextPred
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15101'
    title: Improving Molecular Pretraining with Complementary Featurizations
    date: Sep 29, 2022
    date_iso: '2022-09-29'
    date_display: Sep 2022
    codebase_url: https://github.com/learningmatter-mit/geom
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.702
    metric_stds:
    - 0.02
  - model: CP
    model_plain: CP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.13315'
    title: 3D Molecular Geometry Analysis with 2D Graphs
    date: May 1, 2023
    date_iso: '2023-05-01'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.702
    metric_stds:
    - null
  - model: ECFP-4 + RF
    model_plain: ECFP-4 + RF
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
    - 0.706
    metric_stds:
    - 0.011
  - model: MOCO
    model_plain: MOCO
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2209.15101'
    title: Improving Molecular Pretraining with Complementary Featurizations
    date: Sep 29, 2022
    date_iso: '2022-09-29'
    date_display: Sep 2022
    codebase_url: https://github.com/learningmatter-mit/geom
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.707
    metric_stds:
    - 0.001
  - model: JOAO
    model_plain: JOAO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15101'
    title: Improving Molecular Pretraining with Complementary Featurizations
    date: Sep 29, 2022
    date_iso: '2022-09-29'
    date_display: Sep 2022
    codebase_url: https://github.com/learningmatter-mit/geom
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.708
    metric_stds:
    - 0.007
  - model: GraphConv
    model_plain: GraphConv
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.712
    metric_stds:
    - 0.049
  - model: GraphCL
    model_plain: GraphCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.714
    metric_stds:
    - 0.011
  - model: GCN + JK concat
    model_plain: GCN + JK concat
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.03666'
    title: Application of Graph Neural Networks and graph descriptors for graph classification
    date: Nov 7, 2022
    date_iso: '2022-11-07'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.715
    metric_stds:
    - null
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
    - 0.715
    metric_stds:
    - 0.035
  - model: GraphMVP
    model_plain: GraphMVP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15101'
    title: Improving Molecular Pretraining with Complementary Featurizations
    date: Sep 29, 2022
    date_iso: '2022-09-29'
    date_display: Sep 2022
    codebase_url: https://github.com/learningmatter-mit/geom
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.718
    metric_stds:
    - 0.016
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
    - 0.719
    metric_stds:
    - 0.031
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
    - 0.72
    metric_stds:
    - 0.039
  - model: GCN + JK LSTM
    model_plain: GCN + JK LSTM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.03666'
    title: Application of Graph Neural Networks and graph descriptors for graph classification
    date: Nov 7, 2022
    date_iso: '2022-11-07'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.721
    metric_stds:
    - null
  - model: GraphSAGE + JK LSTM
    model_plain: GraphSAGE + JK LSTM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.03666'
    title: Application of Graph Neural Networks and graph descriptors for graph classification
    date: Nov 7, 2022
    date_iso: '2022-11-07'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.726
    metric_stds:
    - null
  - model: AttrMask
    model_plain: AttrMask
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15101'
    title: Improving Molecular Pretraining with Complementary Featurizations
    date: Sep 29, 2022
    date_iso: '2022-09-29'
    date_display: Sep 2022
    codebase_url: https://github.com/learningmatter-mit/geom
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.73
    metric_stds:
    - 0.004
  - model: AM
    model_plain: AM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.13315'
    title: 3D Molecular Geometry Analysis with 2D Graphs
    date: May 1, 2023
    date_iso: '2023-05-01'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.73
    metric_stds:
    - null
  - model: GraphSAGE + JK concat
    model_plain: GraphSAGE + JK concat
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.03666'
    title: Application of Graph Neural Networks and graph descriptors for graph classification
    date: Nov 7, 2022
    date_iso: '2022-11-07'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.732
    metric_stds:
    - null
  - model: GAP-EMPNN
    model_plain: GAP-EMPNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.13315'
    title: 3D Molecular Geometry Analysis with 2D Graphs
    date: May 1, 2023
    date_iso: '2023-05-01'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.732
    metric_stds:
    - 0.005
  - model: GAT + JK max
    model_plain: GAT + JK max
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.03666'
    title: Application of Graph Neural Networks and graph descriptors for graph classification
    date: Nov 7, 2022
    date_iso: '2022-11-07'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.734
    metric_stds:
    - null
  - model: GIN + JK LSTM
    model_plain: GIN + JK LSTM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.03666'
    title: Application of Graph Neural Networks and graph descriptors for graph classification
    date: Nov 7, 2022
    date_iso: '2022-11-07'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.735
    metric_stds:
    - null
  - model: '---'
    model_plain: '---'
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2209.15101'
    title: Improving Molecular Pretraining with Complementary Featurizations
    date: Sep 29, 2022
    date_iso: '2022-09-29'
    date_display: Sep 2022
    codebase_url: https://github.com/learningmatter-mit/geom
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.736
    metric_stds:
    - 0.006
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
    - 0.738
    metric_stds:
    - null
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
    - 0.738
    metric_stds:
    - 0.025
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
    - 0.742
    metric_stds:
    - null
  - model: EM-GCN
    model_plain: EM-GCN*
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.16401'
    title: Graph Neural Networks with a Distribution of Parametrized Graphs
    date: Oct 25, 2023
    date_iso: '2023-10-25'
    date_display: Oct 2023
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.743
    metric_stds:
    - 0.013
  - model: GIN + JK max
    model_plain: GIN + JK max
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.03666'
    title: Application of Graph Neural Networks and graph descriptors for graph classification
    date: Nov 7, 2022
    date_iso: '2022-11-07'
    date_display: Nov 2022
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
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.03666'
    title: Application of Graph Neural Networks and graph descriptors for graph classification
    date: Nov 7, 2022
    date_iso: '2022-11-07'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.753
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
    arxiv_id: '2310.16401'
    title: Graph Neural Networks with a Distribution of Parametrized Graphs
    date: Oct 25, 2023
    date_iso: '2023-10-25'
    date_display: Oct 2023
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.76
    metric_stds:
    - 0.009
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
    - 0.761
    metric_stds:
    - null
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
    - 0.762
    metric_stds:
    - 0.042
  - model: AttentiveFP
    model_plain: AttentiveFP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.16401'
    title: Graph Neural Networks with a Distribution of Parametrized Graphs
    date: Oct 25, 2023
    date_iso: '2023-10-25'
    date_display: Oct 2023
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.762
    metric_stds:
    - 0.022
  - model: GCN + JK max
    model_plain: GCN + JK max
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.03666'
    title: Application of Graph Neural Networks and graph descriptors for graph classification
    date: Nov 7, 2022
    date_iso: '2022-11-07'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.763
    metric_stds:
    - null
  - model: SimSGT
    model_plain: SimSGT
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
    - 0.771
    metric_stds:
    - 0.041
  - model: MoAMa
    model_plain: MoAMa
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.04589'
    title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    date: Sep 8, 2023
    date_iso: '2023-09-08'
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
    - 0.772
    metric_stds:
    - 0.03
  row_count: 123
  rows_json: /data/datasets/lipophilicity/scaffold-split-rows.json
  chart_json: /data/datasets/lipophilicity/scaffold-split-chart.json
  arch_counts:
    gnn: 73
    hybrid: 30
    graph_transformer: 2
    llm: 0
    walk: 0
    traditional: 18
  metric_counts:
  - 123
  milestones: &id001
  - value: 0.655
    std: 0.036
    model: GC
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: '2017-03-02'
  - value: 0.556
    std: 0.023
    model: MemGNN
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: '2020-02-21'
  milestones_by_metric:
    RMSE: *id001
---

