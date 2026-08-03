---
title: QM7b
slug: qm7b
benchmark: Quantum Chemistry
task_type: graph_regression
description: Quantum chemistry regression on 7,211 molecules (14 electronic and thermodynamic
  targets).
primary_metric: MAE
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.QM7b.html
stats: null
result_count: 98
best_model:
  model: DTNN
  value: 0.074
  metric: MAE
  arxiv_id: '1703.00564'
  paper_title: MoleculeNet
papers:
- arxiv_id: '2502.12638'
  title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation'
  date_iso: '2025-02-18'
  venue: ICLR 2025
- arxiv_id: '2406.13265'
  title: Molecule Graph Networks with Many-body Equivariant Interactions
  date_iso: '2024-06-19'
  venue: ''
- arxiv_id: '2405.10642'
  title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
  date_iso: '2024-05-17'
  venue: ''
- arxiv_id: '2310.20519'
  title: Enhancing Graph Neural Networks with Quantum Computed Encodings
  date_iso: '2023-10-31'
  venue: ''
- arxiv_id: '2310.14753'
  title: Rethinking Tokenizer and Decoder in Masked Graph Modeling for Molecules
  date_iso: '2023-10-23'
  venue: NeurIPS 2023
- arxiv_id: '2310.02232'
  title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
  date_iso: '2023-10-03'
  venue: ICLR 2023
- arxiv_id: '2205.07266'
  title: Discovering the Representation Bottleneck of Graph Neural Networks
  date_iso: '2022-05-15'
  venue: ''
- arxiv_id: '2202.09346'
  title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation and
    Decomposed Fragment Contrast
  date_iso: '2022-02-18'
  venue: ''
- arxiv_id: '2110.01191'
  title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
  date_iso: '2021-10-04'
  venue: AAAI 2021
- arxiv_id: '2106.06130'
  title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
    Prediction'
  date_iso: '2021-06-11'
  venue: ''
- arxiv_id: '2102.06986'
  title: How Framelets Enhance Graph Neural Networks
  date_iso: '2021-02-13'
  venue: ICML 2021
- arxiv_id: '2007.11202'
  title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for Graph Representation
    and Learning'
  date_iso: '2020-07-22'
  venue: ''
- arxiv_id: '1907.04786'
  title: Fast Haar Transforms for Graph Neural Networks
  date_iso: '2019-07-10'
  venue: ''
- arxiv_id: '1703.00564'
  title: MoleculeNet
  date_iso: '2017-03-02'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MAE
  default_metric: MAE
  higher_is_better: false
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - MAE
  - MSE
  - RMSE
  metric_display_names:
  - MAE
  - MSE
  - RMSE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: DTNN
    model_plain: DTNN
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.074
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: Multitask(CM)
    model_plain: Multitask(CM)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    - 0.086
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: KRR(CM)
    model_plain: KRR(CM)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    - 0.098
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: ANI-1
    model_plain: ANI-1
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
    - 2.86
    - null
    - null
    metric_stds:
    - 0.25
    - null
    - null
  - model: DTNN
    model_plain: DTNN
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
    date_iso: '2019-07-10'
    date_display: Jul 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 8.8
    - null
    - null
    metric_stds:
    - 3.5
    - null
    - null
  - model: HANet
    model_plain: HANet
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
    date_iso: '2019-07-10'
    date_display: Jul 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 9.5
    - null
    - null
    metric_stds:
    - 0.71
    - null
    - null
  - model: KRR(CM)
    model_plain: KRR(CM)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1907.04786'
    title: Fast Haar Transforms for Graph Neural Networks
    date: Jul 10, 2019
    date_iso: '2019-07-10'
    date_display: Jul 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 10.2
    - null
    - null
    metric_stds:
    - 0.3
    - null
    - null
  - model: Multitask(CM)
    model_plain: Multitask(CM)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1907.04786'
    title: Fast Haar Transforms for Graph Neural Networks
    date: Jul 10, 2019
    date_iso: '2019-07-10'
    date_display: Jul 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 10.8
    - null
    - null
    metric_stds:
    - 1.3
    - null
    - null
  - model: GPS (4, 2, 128) LE
    model_plain: GPS (4, 2, 128) LE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 14.03
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: SAGE LE+RW
    model_plain: SAGE LE+RW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 14.13
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GPS LE+RW
    model_plain: GPS LE+RW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 14.66
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GPS LE
    model_plain: GPS LE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 14.68
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: SAGE RW
    model_plain: SAGE RW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 14.97
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GPS (4, 2, 128) Q
    model_plain: GPS (4, 2, 128) Q
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 15.36
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: SAGE Q
    model_plain: SAGE Q
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 15.85
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GPS Q
    model_plain: GPS Q
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 16.15
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GPS RW
    model_plain: GPS RW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 16.18
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GPS (4, 2, 128) RW
    model_plain: GPS (4, 2, 128) RW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 16.45
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: Dir-ResolvNet
    model_plain: Dir-ResolvNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 17.12
    - null
    - null
    metric_stds:
    - 0.63
    - null
    - null
  - model: GPS No PE
    model_plain: GPS No PE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 32.23
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: Molformer
    model_plain: Molformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2205.07266'
    title: Discovering the Representation Bottleneck of Graph Neural Networks
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 34.439
    - null
    - null
    metric_stds:
    - 4.017
    - null
    - null
  - model: GPS (4, 2, 128) No PE
    model_plain: GPS (4, 2, 128) No PE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 34.97
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: SAGE LE
    model_plain: SAGE LE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 36.62
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: DiGCN
    model_plain: DiGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 39.95
    - null
    - null
    metric_stds:
    - 6.23
    - null
    - null
  - model: MathNet
    model_plain: MathNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2007.11202'
    title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for Graph Representation
      and Learning'
    date: Jul 22, 2020
    date_iso: '2020-07-22'
    date_display: Jul 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 42.7
    - null
    - null
    metric_stds:
    - 0.92
    - null
    - null
  - model: Molformer
    model_plain: Molformer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 43.2
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GCNConv+SAGPool
    model_plain: GCNConv+SAGPool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2007.11202'
    title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for Graph Representation
      and Learning'
    date: Jul 22, 2020
    date_iso: '2020-07-22'
    date_display: Jul 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 43.6
    - null
    - null
    metric_stds:
    - 0.98
    - null
    - null
  - model: MagNet
    model_plain: MagNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 45.31
    - null
    - null
    metric_stds:
    - 4.24
    - null
    - null
  - model: Graphtransformer
    model_plain: Graphtransformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 47.8
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: EGNN
    model_plain: EGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07266'
    title: Discovering the Representation Bottleneck of Graph Neural Networks
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 53.134
    - null
    - null
    metric_stds:
    - 2.711
    - null
    - null
  - model: ISGR
    model_plain: ISGR
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07266'
    title: Discovering the Representation Bottleneck of Graph Neural Networks
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 53.134
    - null
    - null
    metric_stds:
    - 2.711
    - null
    - null
  - model: +FA
    model_plain: +FA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07266'
    title: Discovering the Representation Bottleneck of Graph Neural Networks
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 55.288
    - null
    - null
    metric_stds:
    - 3.074
    - null
    - null
  - model: DirGNN
    model_plain: DirGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 59.01
    - null
    - null
    metric_stds:
    - 2.54
    - null
    - null
  - model: +SDRF
    model_plain: +SDRF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07266'
    title: Discovering the Representation Bottleneck of Graph Neural Networks
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 59.921
    - null
    - null
    metric_stds:
    - 3.765
    - null
    - null
  - model: SAGE No PE
    model_plain: SAGE No PE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 60.45
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: +DIGL
    model_plain: +DIGL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07266'
    title: Discovering the Representation Bottleneck of Graph Neural Networks
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 61.028
    - null
    - null
    metric_stds:
    - 3.804
    - null
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
    - 63.5
    - null
    - null
    metric_stds:
    - 1.6
    - null
    - null
  - model: iMolCLR
    model_plain: iMolCLR
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09346'
    title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation
      and Decomposed Fragment Contrast
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 66.3
    - null
    - null
    metric_stds:
    - 2.0
    - null
    - null
  - model: R-MAT
    model_plain: R-MAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 68.6
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: SchNet
    model_plain: SchNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 74.2
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: Hi-GMAE-F
    model_plain: Hi-GMAE-F
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.10642'
    title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    date: May 17, 2024
    date_iso: '2024-05-17'
    date_display: May 2024
    codebase_url: https://github.com/LiuChuang0059/Hi-GMAE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 74.4
    - null
    - null
    metric_stds:
    - 1.9
    - null
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
    arxiv_id: '2310.14753'
    title: Rethinking Tokenizer and Decoder in Masked Graph Modeling for Molecules
    date: Oct 23, 2023
    date_iso: '2023-10-23'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 75.4
    - null
    - null
    metric_stds:
    - 0.7
    - null
    - null
  - model: MGCN
    model_plain: MGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 77.6
    - null
    - null
    metric_stds:
    - null
    - null
    - null
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
    - 77.9
    - null
    - null
    metric_stds:
    - 2.1
    - null
    - null
  - model: GraphMAE
    model_plain: GraphMAE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14753'
    title: Rethinking Tokenizer and Decoder in Masked Graph Modeling for Molecules
    date: Oct 23, 2023
    date_iso: '2023-10-23'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 78.4
    - null
    - null
    metric_stds:
    - 2.3
    - null
    - null
  - model: Mole-BERT
    model_plain: Mole-BERT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14753'
    title: Rethinking Tokenizer and Decoder in Masked Graph Modeling for Molecules
    date: Oct 23, 2023
    date_iso: '2023-10-23'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 79.8
    - null
    - null
    metric_stds:
    - 2.6
    - null
    - null
  - model: GraphCL
    model_plain: GraphCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14753'
    title: Rethinking Tokenizer and Decoder in Masked Graph Modeling for Molecules
    date: Oct 23, 2023
    date_iso: '2023-10-23'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 80.4
    - null
    - null
    metric_stds:
    - 3.3
    - null
    - null
  - model: JOAO
    model_plain: JOAO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.10642'
    title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    date: May 17, 2024
    date_iso: '2024-05-17'
    date_display: May 2024
    codebase_url: https://github.com/LiuChuang0059/Hi-GMAE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 84.3
    - null
    - null
    metric_stds:
    - 2.1
    - null
    - null
  - model: MolCLR
    model_plain: MolCLR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09346'
    title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation
      and Decomposed Fragment Contrast
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 87.2
    - null
    - null
    metric_stds:
    - 2.0
    - null
    - null
  - model: ContextPred
    model_plain: ContextPred
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.10642'
    title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    date: May 17, 2024
    date_iso: '2024-05-17'
    date_display: May 2024
    codebase_url: https://github.com/LiuChuang0059/Hi-GMAE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 88.3
    - null
    - null
    metric_stds:
    - 0.5
    - null
    - null
  row_count: 98
  rows_json: /data/datasets/qm7b/standard-split-rows.json
  chart_json: /data/datasets/qm7b/standard-split-chart.json
  arch_counts:
    gnn: 52
    hybrid: 9
    graph_transformer: 5
    llm: 4
    walk: 1
    traditional: 12
  metric_counts:
  - 71
  - 8
  - 19
  milestones: &id001
  - value: 2.86
    std: 0.25
    model: ANI-1
    arxiv_id: '1907.04786'
    title: Fast Haar Transforms for Graph Neural Networks
    date: '2019-07-10'
  milestones_by_metric:
    MAE: *id001
    MSE:
    - value: 41.67
      std: 0.95
      model: UFGPool-Spectrum
      arxiv_id: '2102.06986'
      title: How Framelets Enhance Graph Neural Networks
      date: '2021-02-13'
    RMSE:
    - value: 58.2
      std: 0.5
      model: Geometry
      arxiv_id: '2106.06130'
      title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for
        Property Prediction'
      date: '2021-06-11'
---

