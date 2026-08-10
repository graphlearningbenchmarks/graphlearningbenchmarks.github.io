---
title: CSL
slug: csl
benchmark: GNNBenchmark
task_type: graph_classification
description: Circular skip link graphs — tests graph isomorphism discrimination (10
  classes).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.GNNBenchmarkDataset.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 10
result_count: 104
best_model:
  model: PPGN
  value: 1.0
  metric: Accuracy
  arxiv_id: '2407.01214'
  paper_title: Revisiting Random Walks for Learning on Graphs
papers:
- arxiv_id: '2510.13615'
  title: 'Message Passing on the Edge: Towards Scalable and Expressive GNNs'
  date_iso: '2025-10-15'
  venue: ''
- arxiv_id: '2505.09361'
  title: Efficient Mixed Precision Quantization in Graph Neural Networks
  date_iso: '2025-05-14'
  venue: ''
- arxiv_id: '2502.16233'
  title: Graph Self-Supervised Learning with Learnable Structural and Positional Encodings
  date_iso: '2025-02-22'
  venue: WWW 2025
- arxiv_id: '2502.01122'
  title: Learning Efficient Positional Encodings with Graph Neural Networks
  date_iso: '2025-02-03'
  venue: ICLR 2025
- arxiv_id: '2501.18739'
  title: 'Beyond Message Passing: Neural Graph Pattern Machine'
  date_iso: '2025-01-30'
  venue: ICML 2025
- arxiv_id: '2412.07407'
  title: 'Towards Graph Foundation Models: A Study on the Generalization of Positional
    and Structural Encodings'
  date_iso: '2024-12-10'
  venue: TMLR 2024
- arxiv_id: '2407.01214'
  title: Revisiting Random Walks for Learning on Graphs
  date_iso: '2024-07-01'
  venue: ICLR 2024
- arxiv_id: '2402.14202'
  title: Comparing Graph Transformers via Positional Encodings
  date_iso: '2024-02-22'
  venue: ICML 2024
- arxiv_id: '2402.02005'
  title: Topology-Informed Graph Transformer
  date_iso: '2024-02-03'
  venue: ''
- arxiv_id: '2401.17752'
  title: 'PF-GNN: Differentiable particle filtering based approximation of universal
    graph representations'
  date_iso: '2024-01-31'
  venue: ICLR 2024
- arxiv_id: '2310.20082'
  title: Efficient Subgraph GNNs by Learning Effective Selection Policies
  date_iso: '2023-10-30'
  venue: ICLR 2023
- arxiv_id: '2310.19142'
  title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
  date_iso: '2023-10-29'
  venue: NeurIPS 2023
- arxiv_id: '2303.10576'
  title: An Efficient Subgraph GNN with Provable Substructure Counting Power
  date_iso: '2023-03-19'
  venue: KDD 2023
- arxiv_id: '2003.00982'
  title: GNNBenchmark
  date_iso: '2023-01-01'
  venue: JMLR 2023
- arxiv_id: '2212.13350'
  title: A Generalization of ViT/MLP-Mixer to Graphs
  date_iso: '2022-12-27'
  venue: ICML 2022
- arxiv_id: '2205.13328'
  title: How Powerful are $K$-hop Message Passing Graph Neural Networks
  date_iso: '2022-05-26'
  venue: NeurIPS 2022
- arxiv_id: '2110.00577'
  title: Reconstruction for Powerful Graph Representations
  date_iso: '2021-10-01'
  venue: NeurIPS 2021
- arxiv_id: '2106.12575'
  title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
  date_iso: '2021-06-23'
  venue: NeurIPS 2021
- arxiv_id: '2005.01214'
  title: Graph Homomorphism Convolution
  date_iso: '2020-05-03'
  venue: ICML 2020
- arxiv_id: '1905.12560'
  title: On the Equivalence between Graph Isomorphism Testing and Function Approximation
    with GNNs
  date_iso: '2019-05-29'
  venue: NeurIPS 2019
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 10
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: PPGN
    model_plain: PPGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_iso: '2024-07-01'
    date_display: Jul 2024
    codebase_url: https://github.com/jw9730/random-walk
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: RW-AgentNet
    model_plain: RW-AgentNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_iso: '2024-07-01'
    date_display: Jul 2024
    codebase_url: https://github.com/jw9730/random-walk
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: AgentNet
    model_plain: AgentNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_iso: '2024-07-01'
    date_display: Jul 2024
    codebase_url: https://github.com/jw9730/random-walk
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: CRaWl
    model_plain: CRaWl
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_iso: '2024-07-01'
    date_display: Jul 2024
    codebase_url: https://github.com/jw9730/random-walk
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: RWNN-DeBERTa
    model_plain: RWNN-DeBERTa
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_iso: '2024-07-01'
    date_display: Jul 2024
    codebase_url: https://github.com/jw9730/random-walk
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: GHC-Cycles
    model_plain: GHC-Cycles
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2005.01214'
    title: Graph Homomorphism Convolution
    date: May 3, 2020
    date_iso: '2020-05-03'
    date_display: May 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: KP-GIN
    model_plain: KP-GIN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.13328'
    title: How Powerful are $K$-hop Message Passing Graph Neural Networks
    date: May 26, 2022
    date_iso: '2022-05-26'
    date_display: May 2022
    codebase_url: https://github.com/JiaruiFeng/KP-GNN
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: Reconstr. (n-1)
    model_plain: Reconstr. (n-1)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2110.00577'
    title: Reconstruction for Powerful Graph Representations
    date: Oct 1, 2021
    date_iso: '2021-10-01'
    date_display: Oct 2021
    codebase_url: https://github.com/PurdueMINDS/reconstruction-gnns
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: NGNN
    model_plain: NGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.19142'
    title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/LechengKong/MAG-GNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: GNNAK+
    model_plain: GNNAK+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.19142'
    title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/LechengKong/MAG-GNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: SSWL+
    model_plain: SSWL+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.19142'
    title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/LechengKong/MAG-GNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: RNM
    model_plain: RNM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.19142'
    title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/LechengKong/MAG-GNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: I^2GNN
    model_plain: I^2GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.19142'
    title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/LechengKong/MAG-GNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: MAG-GNN
    model_plain: MAG-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.19142'
    title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/LechengKong/MAG-GNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: Full
    model_plain: Full
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.20082'
    title: Efficient Subgraph GNNs by Learning Effective Selection Policies
    date: Oct 30, 2023
    date_iso: '2023-10-30'
    date_display: Oct 2023
    codebase_url: https://github.com/beabevi/policy-learn
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: Random T=2
    model_plain: Random T=2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.20082'
    title: Efficient Subgraph GNNs by Learning Effective Selection Policies
    date: Oct 30, 2023
    date_iso: '2023-10-30'
    date_display: Oct 2023
    codebase_url: https://github.com/beabevi/policy-learn
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: MPNNs
    model_plain: MPNNs
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.20082'
    title: Efficient Subgraph GNNs by Learning Effective Selection Policies
    date: Oct 30, 2023
    date_iso: '2023-10-30'
    date_display: Oct 2023
    codebase_url: https://github.com/beabevi/policy-learn
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: I^2-GNN
    model_plain: I^2-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.10576'
    title: An Efficient Subgraph GNN with Provable Substructure Counting Power
    date: Mar 19, 2023
    date_iso: '2023-03-19'
    date_display: Mar 2023
    codebase_url: https://github.com/pkuyzy/ESC-GNN
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: ESC-GNN
    model_plain: ESC-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.10576'
    title: An Efficient Subgraph GNN with Provable Substructure Counting Power
    date: Mar 19, 2023
    date_iso: '2023-03-19'
    date_display: Mar 2023
    codebase_url: https://github.com/pkuyzy/ESC-GNN
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: PF-GNN
    model_plain: PF-GNN
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
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: APE-GT
    model_plain: APE-GT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.14202'
    title: Comparing Graph Transformers via Positional Encodings
    date: Feb 22, 2024
    date_iso: '2024-02-22'
    date_display: Feb 2024
    codebase_url: https://github.com/blackmit/comparing_graph_transformers_via_positional_encodings
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: DeepSet RPE-GT
    model_plain: DeepSet RPE-GT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.14202'
    title: Comparing Graph Transformers via Positional Encodings
    date: Feb 22, 2024
    date_iso: '2024-02-22'
    date_display: Feb 2024
    codebase_url: https://github.com/blackmit/comparing_graph_transformers_via_positional_encodings
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: RPE-augWL
    model_plain: RPE-augWL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.14202'
    title: Comparing Graph Transformers via Positional Encodings
    date: Feb 22, 2024
    date_iso: '2024-02-22'
    date_display: Feb 2024
    codebase_url: https://github.com/blackmit/comparing_graph_transformers_via_positional_encodings
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: EGN APE-GT
    model_plain: EGN APE-GT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.14202'
    title: Comparing Graph Transformers via Positional Encodings
    date: Feb 22, 2024
    date_iso: '2024-02-22'
    date_display: Feb 2024
    codebase_url: https://github.com/blackmit/comparing_graph_transformers_via_positional_encodings
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: GPS+LapPE+RWSE (1 layer)
    model_plain: GPS+LapPE+RWSE (1 layer)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: TIGT
    model_plain: TIGT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - 0.0
  - model: B-PEARL
    model_plain: B-PEARL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.01122'
    title: Learning Efficient Positional Encodings with Graph Neural Networks
    date: Feb 3, 2025
    date_iso: '2025-02-03'
    date_display: Feb 2025
    codebase_url: https://github.com/ehejin/Pearl-PE
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: R-PEARL
    model_plain: R-PEARL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.01122'
    title: Learning Efficient Positional Encodings with Graph Neural Networks
    date: Feb 3, 2025
    date_iso: '2025-02-03'
    date_display: Feb 2025
    codebase_url: https://github.com/ehejin/Pearl-PE
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: Graph ViT/MLP-Mixer
    model_plain: Graph ViT/MLP-Mixer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2212.13350'
    title: A Generalization of ViT/MLP-Mixer to Graphs
    date: Dec 27, 2022
    date_iso: '2022-12-27'
    date_display: Dec 2022
    codebase_url: https://github.com/XiaoxinHe/Graph-ViT-MLPMixer
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: Graph ViT
    model_plain: Graph ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2501.18739'
    title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    date: Jan 30, 2025
    date_iso: '2025-01-30'
    date_display: Jan 2025
    codebase_url: https://github.com/Zehong-Wang/GPM
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: GPM
    model_plain: GPM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2501.18739'
    title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    date: Jan 30, 2025
    date_iso: '2025-01-30'
    date_display: Jan 2025
    codebase_url: https://github.com/Zehong-Wang/GPM
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: MoNet
    model_plain: MoNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.99967
    metric_stds:
    - 0.00332
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.99933
    metric_stds:
    - 0.00467
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.99933
    metric_stds:
    - 0.00467
  - model: GatedGCN (Rand sign(EigVecs))
    model_plain: GatedGCN (Rand sign(EigVecs))
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.99767
    metric_stds:
    - 0.00394
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.996
    metric_stds:
    - 0.01083
  - model: GatedGCN (Abs(EigVecs))
    model_plain: GatedGCN (Abs(EigVecs))
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.99433
    metric_stds:
    - 0.01133
  - model: FP32
    model_plain: FP32
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.09361'
    title: Efficient Mixed Precision Quantization in Graph Neural Networks
    date: May 14, 2025
    date_iso: '2025-05-14'
    date_display: May 2025
    codebase_url: https://github.com/SamirMoustafa/MixQ
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.994
    metric_stds:
    - 0.013
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.99333
    metric_stds:
    - 0.01333
  - model: Positional GIN
    model_plain: Positional GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.00577'
    title: Reconstruction for Powerful Graph Representations
    date: Oct 1, 2021
    date_iso: '2021-10-01'
    date_display: Oct 2021
    codebase_url: https://github.com/PurdueMINDS/reconstruction-gnns
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9933
    metric_stds:
    - 0.0133
  - model: StructPosGSSL-SA
    model_plain: StructPosGSSL-SA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.16233'
    title: Graph Self-Supervised Learning with Learnable Structural and Positional
      Encodings
    date: Feb 22, 2025
    date_iso: '2025-02-22'
    date_display: Feb 2025
    codebase_url: https://github.com/wokas36/StructPosGSSL
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.986
    metric_stds:
    - 0.028
  - model: Cy2C-GIN-1
    model_plain: Cy2C-GIN-1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9833
    metric_stds:
    - 0.0333
  - model: StructPosGSSL-FA
    model_plain: StructPosGSSL-FA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.16233'
    title: Graph Self-Supervised Learning with Learnable Structural and Positional
      Encodings
    date: Feb 22, 2025
    date_iso: '2025-02-22'
    date_display: Feb 2025
    codebase_url: https://github.com/wokas36/StructPosGSSL
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.983
    metric_stds:
    - 0.025
  - model: PPGN (3-WL)
    model_plain: PPGN (3-WL)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.00577'
    title: Reconstruction for Powerful Graph Representations
    date: Oct 1, 2021
    date_iso: '2021-10-01'
    date_display: Oct 2021
    codebase_url: https://github.com/PurdueMINDS/reconstruction-gnns
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.978
    metric_stds:
    - 0.1091
  - model: 3-WL GNN
    model_plain: 3-WL GNN
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
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.978
    metric_stds:
    - 0.109
  - model: 3WLGNN
    model_plain: 3WLGNN
    is_baseline: true
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.978
    metric_stds:
    - 0.10916
  - model: 3-GCN
    model_plain: 3-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.16233'
    title: Graph Self-Supervised Learning with Learnable Structural and Positional
      Encodings
    date: Feb 22, 2025
    date_iso: '2025-02-22'
    date_display: Feb 2025
    codebase_url: https://github.com/wokas36/StructPosGSSL
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.957
    metric_stds:
    - 0.148
  - model: 3-GNN
    model_plain: 3-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.10576'
    title: An Efficient Subgraph GNN with Provable Substructure Counting Power
    date: Mar 19, 2023
    date_iso: '2023-03-19'
    date_display: Mar 2023
    codebase_url: https://github.com/pkuyzy/ESC-GNN
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.957
    metric_stds:
    - null
  row_count: 104
  rows_json: /data/datasets/csl/standard-split-rows.json
  chart_json: /data/datasets/csl/standard-split-chart.json
  arch_counts:
    gnn: 74
    hybrid: 8
    graph_transformer: 9
    llm: 0
    walk: 1
    traditional: 6
  metric_counts:
  - 104
  milestones: &id001
  - value: 0.8
    std: 0.0
    model: sGNN_5
    arxiv_id: '1905.12560'
    title: On the Equivalence between Graph Isomorphism Testing and Function Approximation
      with GNNs
    date: '2019-05-29'
  - value: 1.0
    std: 0.0
    model: GHC-Cycles
    arxiv_id: '2005.01214'
    title: Graph Homomorphism Convolution
    date: '2020-05-03'
  milestones_by_metric:
    Accuracy: *id001
---

