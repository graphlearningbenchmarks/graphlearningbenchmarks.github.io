---
title: RDT-B
slug: rdt-b
benchmark: TU Dortmund
task_type: graph_classification
short_description: Classify Reddit threads as question-answering or discussion; this
  is an alias of REDDIT-BINARY.
description: '**2-class graph classification** Alias for REDDIT-BINARY in some papers.
  Uses the released node/edge labels or attributes; several social datasets are featureless.
  No canonical split; report folds and any added node features. Evaluated by Accuracy.'
detailed_description:
  task: Alias for REDDIT-BINARY in some papers. The primary catalog metric is Accuracy.
  data: Alias for REDDIT-BINARY in some papers. The cataloged artifact reports 2,000
    graphs, 2 target classes or tasks.
  features: The TU text format may contain discrete node or edge labels and optional
    continuous attributes. Social-network datasets commonly have no intrinsic node
    attributes, so papers often add constant or degree features; that choice changes
    the input.
  splits_and_evaluation: 'The catalog records these protocols or variants: 10-fold
    CV. Evaluation uses Accuracy (higher is better). Exact masks or folds must come
    from the cited release.'
  quirks_and_pitfalls: TU datasets have no canonical train/test split. Report cross-validation
    folds, seeds, feature construction, and whether duplicate or isomorphic graphs
    were removed; published results can otherwise differ for protocol rather than
    model quality.
sources:
- title: TU Dortmund benchmark
  arxiv_id: '2007.08663'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric RDT-B loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
stats:
  num_graphs: 2000
  avg_nodes: 429.63
  avg_edges: 497.75
  num_classes: 2
result_count: 108
best_model:
  model: OEPG
  value: 0.963
  metric: Accuracy
  arxiv_id: '2205.15746'
  paper_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
    Learning
papers:
- arxiv_id: '2506.06212'
  title: Model-Driven Graph Contrastive Learning
  date_iso: '2025-06-06'
  venue: ''
- arxiv_id: '2505.19024'
  title: Learn Beneficial Noise as Graph Augmentation
  date_iso: '2025-05-25'
  venue: ICML 2025
- arxiv_id: '2505.15015'
  title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
  date_iso: '2025-05-21'
  venue: ''
- arxiv_id: '2406.08897'
  title: Motif-driven Subgraph Structure Learning for Graph Classification
  date_iso: '2024-06-13'
  venue: ''
- arxiv_id: '2406.00403'
  title: Dual-perspective Cross Contrastive Learning in Graph Transformers
  date_iso: '2024-06-01'
  venue: ''
- arxiv_id: '2405.01350'
  title: Community-Invariant Graph Contrastive Learning
  date_iso: '2024-05-02'
  venue: ICML 2024
- arxiv_id: '2401.17580'
  title: Graph Contrastive Learning with Cohesive Subgraph Awareness
  date_iso: '2024-01-31'
  venue: WWW 2024
- arxiv_id: '2309.02304'
  title: Graph Self-Contrast Representation Learning
  date_iso: '2023-09-05'
  venue: ''
- arxiv_id: '2307.01053'
  title: 'ENGAGE: Explanation Guided Data Augmentation for Graph Representation Learning'
  date_iso: '2023-07-03'
  venue: ''
- arxiv_id: '2305.06102'
  title: Towards Better Graph Representation Learning with Parameterized Decomposition
    & Filtering
  date_iso: '2023-05-10'
  venue: ICML 2023
- arxiv_id: '2209.06560'
  title: Graph Contrastive Learning with Personalized Augmentation
  date_iso: '2022-09-14'
  venue: ''
- arxiv_id: '2206.11010'
  title: Agent-based Graph Neural Networks
  date_iso: '2022-06-22'
  venue: ICLR 2022
- arxiv_id: '2206.07869'
  title: Let Invariant Rationale Discovery Inspire Graph Contrastive Learning
  date_iso: '2022-06-16'
  venue: ICML 2022
- arxiv_id: '2205.15746'
  title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
    Learning
  date_iso: '2022-05-31'
  venue: ICML 2022
- arxiv_id: '2202.08333'
  title: Self-Supervised Representation Learning via Latent Graph Prediction
  date_iso: '2022-02-16'
  venue: ICML 2022
- arxiv_id: '2202.03104'
  title: 'SimGRACE: A Simple Framework for Graph Contrastive Learning without Data
    Augmentation'
  date_iso: '2022-02-07'
  venue: WWW 2022
- arxiv_id: '2110.03753'
  title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
  date_iso: '2021-10-07'
  venue: ICLR 2021
- arxiv_id: '2106.12575'
  title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
  date_iso: '2021-06-23'
  venue: NeurIPS 2021
- arxiv_id: '2106.09645'
  title: Prototypical Graph Contrastive Learning
  date_iso: '2021-06-17'
  venue: ''
- arxiv_id: '2106.05819'
  title: Adversarial Graph Augmentation to Improve Graph Contrastive Learning
  date_iso: '2021-06-10'
  venue: NeurIPS 2021
- arxiv_id: '2106.07594'
  title: Graph Contrastive Learning Automated
  date_iso: '2021-06-10'
  venue: ICML 2021
- arxiv_id: '2103.03212'
  title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial Networks'
  date_iso: '2021-03-04'
  venue: ICML 2021
- arxiv_id: '2103.00111'
  title: 'Graph Self-Supervised Learning: A Survey'
  date_iso: '2021-02-27'
  venue: ''
- arxiv_id: '2009.03294'
  title: 'GraphNorm: A Principled Approach to Accelerating Graph Neural Network Training'
  date_iso: '2020-09-07'
  venue: ICML 2020
- arxiv_id: '1810.00826'
  title: How Powerful are Graph Neural Networks?
  date_iso: '2018-10-01'
  venue: ICLR 2018
variants:
- slug: 10-fold-cv
  name: 10-fold CV
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 2000
    avg_nodes: 429.63
    avg_edges: 497.75
    num_classes: 2
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: OEPG
    model_plain: OEPG
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15746'
    title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
      Learning
    date: May 31, 2022
    date_iso: '2022-05-31'
    date_display: May 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.963
    metric_stds:
    - 0.009
  - model: MSH-GNN
    model_plain: MSH-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_iso: '2025-05-21'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.958
    metric_stds:
    - 0.009
  - model: GNN-AK+
    model_plain: GNN-AK+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: Oct 7, 2021
    date_iso: '2021-10-07'
    date_display: Oct 2021
    codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.948
    metric_stds:
    - 0.008
  - model: AgentNet
    model_plain: AgentNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.11010'
    title: Agent-based Graph Neural Networks
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/KarolisMart/AgentNet
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.942
    metric_stds:
    - 0.012
  - model: GraphNorm
    model_plain: GraphNorm
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.03294'
    title: 'GraphNorm: A Principled Approach to Accelerating Graph Neural Network
      Training'
    date: Sep 7, 2020
    date_iso: '2020-09-07'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.935
    metric_stds:
    - 0.021
  - model: GSO
    model_plain: GSO
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.06102'
    title: Towards Better Graph Representation Learning with Parameterized Decomposition
      & Filtering
    date: May 10, 2023
    date_iso: '2023-05-10'
    date_display: May 2023
    codebase_url: https://github.com/qslim/PDF
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.934
    metric_stds:
    - 0.013
  - model: ESAN
    model_plain: ESAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.11010'
    title: Agent-based Graph Neural Networks
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/KarolisMart/AgentNet
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.933
    metric_stds:
    - 0.013
  - model: GIN + InstanceNorm
    model_plain: GIN + InstanceNorm
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.03294'
    title: 'GraphNorm: A Principled Approach to Accelerating Graph Neural Network
      Training'
    date: Sep 7, 2020
    date_iso: '2020-09-07'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.932
    metric_stds:
    - 0.017
  - model: CRaWl
    model_plain: CRaWl
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.11010'
    title: Agent-based Graph Neural Networks
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/KarolisMart/AgentNet
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.928
    metric_stds:
    - 0.022
  - model: Wit-TopoPool
    model_plain: Wit-TopoPool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_iso: '2025-05-21'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.928
    metric_stds:
    - 0.011
  - model: DGCL
    model_plain: DGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.15746'
    title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
      Learning
    date: May 31, 2022
    date_iso: '2022-05-31'
    date_display: May 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.927
    metric_stds:
    - 0.002
  - model: GIN-0
    model_plain: GIN-0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.09645'
    title: Prototypical Graph Contrastive Learning
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/ha-lins/PGCL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.924
    metric_stds:
    - 0.025
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.00111'
    title: 'Graph Self-Supervised Learning: A Survey'
    date: Feb 27, 2021
    date_iso: '2021-02-27'
    date_display: Feb 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.924
    metric_stds:
    - null
  - model: GIN + BatchNorm
    model_plain: GIN + BatchNorm
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.03294'
    title: 'GraphNorm: A Principled Approach to Accelerating Graph Neural Network
      Training'
    date: Sep 7, 2020
    date_iso: '2020-09-07'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.924
    metric_stds:
    - 0.025
  - model: CIN
    model_plain: CIN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.12575'
    title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    date: Jun 23, 2021
    date_iso: '2021-06-23'
    date_display: Jun 2021
    codebase_url: https://github.com/twitter-research/cwn
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.924
    metric_stds:
    - 0.021
  - model: Sum--MLP (GIN-0)
    model_plain: Sum--MLP (GIN-0)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1810.00826'
    title: How Powerful are Graph Neural Networks?
    date: Oct 1, 2018
    date_iso: '2018-10-01'
    date_display: Oct 2018
    codebase_url: https://github.com/weihua916/powerful-gnns
    published_conference: ICLR 2018
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2018
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.924
    metric_stds:
    - 0.025
  - model: AD-GCL-OPT
    model_plain: AD-GCL-OPT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.05819'
    title: Adversarial Graph Augmentation to Improve Graph Contrastive Learning
    date: Jun 10, 2021
    date_iso: '2021-06-10'
    date_display: Jun 2021
    codebase_url: https://github.com/susheels/adgcl
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9235
    metric_stds:
    - 0.0042
  - model: CTAug-GraphCL
    model_plain: CTAug-GraphCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.17580'
    title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/wuyucheng2002/CTAug
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9228
    metric_stds:
    - 0.0033
  - model: GIN-ε
    model_plain: GIN-ε
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.09645'
    title: Prototypical Graph Contrastive Learning
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/ha-lins/PGCL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.922
    metric_stds:
    - 0.023
  - model: SIN
    model_plain: SIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.03212'
    title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial Networks'
    date: Mar 4, 2021
    date_iso: '2021-03-04'
    date_display: Mar 2021
    codebase_url: ''
    published_conference: ICML 2021
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.922
    metric_stds:
    - 0.01
  - model: CTAug-JOAO
    model_plain: CTAug-JOAO
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.17580'
    title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/wuyucheng2002/CTAug
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9219
    metric_stds:
    - 0.0024
  - model: AD-GCL-FIX
    model_plain: AD-GCL-FIX
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.05819'
    title: Adversarial Graph Augmentation to Improve Graph Contrastive Learning
    date: Jun 10, 2021
    date_iso: '2021-06-10'
    date_display: Jun 2021
    codebase_url: https://github.com/susheels/adgcl
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9206
    metric_stds:
    - 0.0042
  - model: GraphCL
    model_plain: GraphCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17580'
    title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/wuyucheng2002/CTAug
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9169
    metric_stds:
    - 0.007
  - model: JOAO
    model_plain: JOAO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17580'
    title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/wuyucheng2002/CTAug
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9166
    metric_stds:
    - 0.0059
  - model: PGCL
    model_plain: PGCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2106.09645'
    title: Prototypical Graph Contrastive Learning
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/ha-lins/PGCL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.915
    metric_stds:
    - 0.007
  - model: RGCL
    model_plain: RGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17580'
    title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/wuyucheng2002/CTAug
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9138
    metric_stds:
    - 0.004
  - model: HTC
    model_plain: HTC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.00111'
    title: 'Graph Self-Supervised Learning: A Survey'
    date: Feb 27, 2021
    date_iso: '2021-02-27'
    date_display: Feb 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.913
    metric_stds:
    - null
  - model: GraphSC
    model_plain: GraphSC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.02304'
    title: Graph Self-Contrast Representation Learning
    date: Sep 5, 2023
    date_iso: '2023-09-05'
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
    - 0.9108
    metric_stds:
    - 0.0056
  - model: DC-GCL
    model_plain: DC-GCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.00403'
    title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    date: Jun 1, 2024
    date_iso: '2024-06-01'
    date_display: Jun 2024
    codebase_url: https://github.com/Celin-Yao/DC-GCL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9104
    metric_stds:
    - 0.0045
  - model: CI-GCL
    model_plain: CI-GCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.01350'
    title: Community-Invariant Graph Contrastive Learning
    date: May 2, 2024
    date_iso: '2024-05-02'
    date_display: May 2024
    codebase_url: https://github.com/ShiyinTan/CI-GCL.git
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.908
    metric_stds:
    - 0.005
  - model: DRGCL
    model_plain: DRGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.00403'
    title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    date: Jun 1, 2024
    date_iso: '2024-06-01'
    date_display: Jun 2024
    codebase_url: https://github.com/Celin-Yao/DC-GCL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.908
    metric_stds:
    - 0.003
  - model: EG-SimCLR
    model_plain: EG-SimCLR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.01053'
    title: 'ENGAGE: Explanation Guided Data Augmentation for Graph Representation
      Learning'
    date: Jul 3, 2023
    date_iso: '2023-07-03'
    date_display: Jul 2023
    codebase_url: https://github.com/sycny/ENGAGE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.907
    metric_stds:
    - 0.0046
  - model: LaGraph
    model_plain: LaGraph
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.08333'
    title: Self-Supervised Representation Learning via Latent Graph Prediction
    date: Feb 16, 2022
    date_iso: '2022-02-16'
    date_display: Feb 2022
    codebase_url: https://github.com/divelab/DIG
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.904
    metric_stds:
    - 0.008
  - model: RGCL
    model_plain: RGCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.07869'
    title: Let Invariant Rationale Discovery Inspire Graph Contrastive Learning
    date: Jun 16, 2022
    date_iso: '2022-06-16'
    date_display: Jun 2022
    codebase_url: https://github.com/lsh0520/RGCL
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9034
    metric_stds:
    - 0.0058
  - model: GraphSC-MSE
    model_plain: GraphSC-MSE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.02304'
    title: Graph Self-Contrast Representation Learning
    date: Sep 5, 2023
    date_iso: '2023-09-05'
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
    - 0.9026
    metric_stds:
    - 0.008
  - model: MGCL
    model_plain: MGCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.06212'
    title: Model-Driven Graph Contrastive Learning
    date: Jun 6, 2025
    date_iso: '2025-06-06'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9025
    metric_stds:
    - 0.0039
  - model: SEGA
    model_plain: SEGA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.01350'
    title: Community-Invariant Graph Contrastive Learning
    date: May 2, 2024
    date_iso: '2024-05-02'
    date_display: May 2024
    codebase_url: https://github.com/ShiyinTan/CI-GCL.git
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9021
    metric_stds:
    - 0.007
  - model: AD-GCL
    model_plain: AD-GCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.07869'
    title: Let Invariant Rationale Discovery Inspire Graph Contrastive Learning
    date: Jun 16, 2022
    date_iso: '2022-06-16'
    date_display: Jun 2022
    codebase_url: https://github.com/lsh0520/RGCL
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9007
    metric_stds:
    - 0.0085
  - model: Sum--1-Layer
    model_plain: Sum--1-Layer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1810.00826'
    title: How Powerful are Graph Neural Networks?
    date: Oct 1, 2018
    date_iso: '2018-10-01'
    date_display: Oct 2018
    codebase_url: https://github.com/weihua916/powerful-gnns
    published_conference: ICLR 2018
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2018
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9
    metric_stds:
    - 0.027
  - model: GPA
    model_plain: GPA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2209.06560'
    title: Graph Contrastive Learning with Personalized Augmentation
    date: Sep 14, 2022
    date_iso: '2022-09-14'
    date_display: Sep 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8999
    metric_stds:
    - 0.0032
  - model: HG-SimCLR
    model_plain: HG-SimCLR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.01053'
    title: 'ENGAGE: Explanation Guided Data Augmentation for Graph Representation
      Learning'
    date: Jul 3, 2023
    date_iso: '2023-07-03'
    date_display: Jul 2023
    codebase_url: https://github.com/sycny/ENGAGE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8992
    metric_stds:
    - 0.0053
  - model: DropGIN
    model_plain: DropGIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.11010'
    title: Agent-based Graph Neural Networks
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/KarolisMart/AgentNet
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.899
    metric_stds:
    - 0.017
  - model: GCC
    model_plain: GCC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.00111'
    title: 'Graph Self-Supervised Learning: A Survey'
    date: Feb 27, 2021
    date_iso: '2021-02-27'
    date_display: Feb 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.898
    metric_stds:
    - null
  - model: HG-Simsiam
    model_plain: HG-Simsiam
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.01053'
    title: 'ENGAGE: Explanation Guided Data Augmentation for Graph Representation
      Learning'
    date: Jul 3, 2023
    date_iso: '2023-07-03'
    date_display: Jul 2023
    codebase_url: https://github.com/sycny/ENGAGE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8963
    metric_stds:
    - 0.0055
  - model: GraphCL
    model_plain: GraphCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.05819'
    title: Adversarial Graph Augmentation to Improve Graph Contrastive Learning
    date: Jun 10, 2021
    date_iso: '2021-06-10'
    date_display: Jun 2021
    codebase_url: https://github.com/susheels/adgcl
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8953
    metric_stds:
    - 0.0084
  - model: SimGRACE
    model_plain: SimGRACE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03104'
    title: 'SimGRACE: A Simple Framework for Graph Contrastive Learning without Data
      Augmentation'
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/junxia97/SimGRACE
    published_conference: WWW 2022
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8951
    metric_stds:
    - 0.0089
  - model: GraphCL(G)
    model_plain: GraphCL(G)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.00111'
    title: 'Graph Self-Supervised Learning: A Survey'
    date: Feb 27, 2021
    date_iso: '2021-02-27'
    date_display: Feb 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.895
    metric_stds:
    - null
  - model: AutoGCL
    model_plain: AutoGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17580'
    title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/wuyucheng2002/CTAug
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8931
    metric_stds:
    - 0.0148
  - model: EG-Simsiam
    model_plain: EG-Simsiam
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.01053'
    title: 'ENGAGE: Explanation Guided Data Augmentation for Graph Representation
      Learning'
    date: Jul 3, 2023
    date_iso: '2023-07-03'
    date_display: Jul 2023
    codebase_url: https://github.com/sycny/ENGAGE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8917
    metric_stds:
    - 0.0043
  - model: JOAOv2
    model_plain: JOAOv2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.05819'
    title: Adversarial Graph Augmentation to Improve Graph Contrastive Learning
    date: Jun 10, 2021
    date_iso: '2021-06-10'
    date_display: Jun 2021
    codebase_url: https://github.com/susheels/adgcl
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8879
    metric_stds:
    - 0.0065
  row_count: 108
  rows_json: /data/datasets/rdt-b/10-fold-cv-rows.json
  chart_json: /data/datasets/rdt-b/10-fold-cv-chart.json
  arch_counts:
    gnn: 74
    hybrid: 17
    graph_transformer: 0
    llm: 0
    walk: 4
    traditional: 13
  metric_counts:
  - 108
  milestones: &id001
  - value: 0.924
    std: 0.025
    model: Sum--MLP (GIN-0)
    arxiv_id: '1810.00826'
    title: How Powerful are Graph Neural Networks?
    date: '2018-10-01'
  - value: 0.935
    std: 0.021
    model: GraphNorm
    arxiv_id: '2009.03294'
    title: 'GraphNorm: A Principled Approach to Accelerating Graph Neural Network
      Training'
    date: '2020-09-07'
  - value: 0.948
    std: 0.008
    model: GNN-AK+
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: '2021-10-07'
  - value: 0.963
    std: 0.009
    model: OEPG
    arxiv_id: '2205.15746'
    title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
      Learning
    date: '2022-05-31'
  milestones_by_metric:
    Accuracy: *id001
---

