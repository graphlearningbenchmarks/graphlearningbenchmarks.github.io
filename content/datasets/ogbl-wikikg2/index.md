---
title: ogbl-wikikg2
slug: ogbl-wikikg2
benchmark: OGB
task_type: link_prediction
short_description: Predict missing heads or tails of Wikidata triples.
description: '**Link prediction** Predict missing heads or tails of Wikidata triples.
  Entities are identifiers with learned representations in the standard task; no text
  or image features are supplied by the core artifact. Evaluated by MRR.'
detailed_description:
  task: Predict missing heads or tails of Wikidata triples. Filtered MRR ranks each
    true entity against 500 sampled corrupt heads and 500 sampled corrupt tails that
    do not form known triples.
  data: The graph contains 2,500,604 retained entities, 535 directed relation types,
    and 17,137,181 triples extracted from historical Wikidata dumps after filtering
    rare entities.
  features: Entities are identifiers with learned representations in the standard
    task; no text or image features are supplied by the core artifact. Relations are
    typed directed edges.
  splits_and_evaluation: Triples in the May 2015 snapshot train the model, additions
    present by August validate it, and additions by November form test. Only entities
    and relation types already present in May are retained.
  quirks_and_pitfalls: Wikidata is incomplete and collaboratively edited, so an absent
    triple is not necessarily false. The predecessor ogbl-wikikg had a negative-sampling
    bug and is deprecated. Sampled MRR differs from ranking all entities, and inverse-relation
    augmentation changes the model input.
sources:
- title: Open Graph Benchmark
  arxiv_id: '2005.00687'
  kind: benchmark_definition
- title: OGB link property prediction documentation
  url: https://ogb.stanford.edu/docs/linkprop/#ogbl-wikikg2
  kind: official_documentation
- title: Wikidata, a free collaborative knowledgebase
  url: https://doi.org/10.1145/2629489
  kind: upstream_data_source
primary_metric: MRR
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGBLinkPropPredDataset.html
stats:
  num_graphs: 1
  avg_nodes: 2500604.0
  avg_edges: 17137181.0
  num_classes: null
  extra_stats:
    avg_degree: 6.853
    degree_convention: derived as avg_edges / avg_nodes for directed knowledge-graph
      triples (average out-degree)
    edge_feature_type: 535 categorical relation types
    label_imbalance: no fixed binary label distribution; relation and entity frequencies
      are not summarized in the canonical OGB documentation
    node_feature_type: no supplied node features; entity IDs are represented by learned
      embeddings
    num_relation_types: 535
    statistic_notes: clustering coefficient and diameter are not reported; relation
      multiplicity and direction are part of the task
result_count: 54
best_model:
  model: InterHT + DigPiece
  value: 0.7293
  metric: MRR
  arxiv_id: '2202.04897'
  paper_title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and
    Tail Entities'
papers:
- arxiv_id: '2506.05393'
  title: Are Large Language Models Good Temporal Graph Learners?
  date_iso: '2025-06-03'
  venue: ''
- arxiv_id: '2412.03783'
  title: 'Expressivity of Representation Learning on Continuous-Time Dynamic Graphs:
    An Information-Flow Centric Review'
  date_iso: '2024-12-05'
  venue: TMLR 2024
- arxiv_id: '2209.08271'
  title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
  date_iso: '2022-09-17'
  venue: ''
- arxiv_id: '2206.04798'
  title: 'A*Net: A Scalable Path-based Reasoning Approach for Knowledge Graphs'
  date_iso: '2022-06-07'
  venue: NeurIPS 2022
- arxiv_id: '2205.14209'
  title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
    Subgraph'
  date_iso: '2022-05-27'
  venue: ICLR 2022
- arxiv_id: '2204.13957'
  title: 'PIE: a Parameter and Inference Efficient Solution for Large Scale Knowledge
    Graph Embedding Reasoning'
  date_iso: '2022-04-29'
  venue: ''
- arxiv_id: '2202.04897'
  title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
    Entities'
  date_iso: '2022-02-10'
  venue: ''
- arxiv_id: '2011.03798'
  title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
  date_iso: '2020-11-07'
  venue: ''
- arxiv_id: '2005.00687'
  title: OGB
  date_iso: '2020-05-02'
  venue: NeurIPS 2020
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MRR
  default_metric: MRR
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 2500604.0
    avg_edges: 17137181.0
    num_classes: null
    extra_stats:
      avg_degree: 6.853
      degree_convention: derived as avg_edges / avg_nodes for directed knowledge-graph
        triples (average out-degree)
      edge_feature_type: 535 categorical relation types
      label_imbalance: no fixed binary label distribution; relation and entity frequencies
        are not summarized in the canonical OGB documentation
      node_feature_type: no supplied node features; entity IDs are represented by
        learned embeddings
      num_relation_types: 535
      statistic_notes: clustering coefficient and diameter are not reported; relation
        multiplicity and direction are part of the task
  metrics:
  - MRR
  metric_display_names:
  - MRR
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: InterHT + DigPiece
    model_plain: InterHT + DigPiece
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7293
    metric_stds:
    - 0.0018
  - model: StarGraph + TripleRE'
    model_plain: StarGraph + TripleRE'
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.729
    metric_stds:
    - null
  - model: TripleRE + StarGraph
    model_plain: TripleRE + StarGraph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 86.7
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7201
    metric_stds:
    - 0.0011
  - model: TNCN
    model_plain: TNCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.711
    metric_stds:
    - 0.007
  - model: TranS(large) + NodePiece
    model_plain: TranS(large) + NodePiece
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 38.430804
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6939
    metric_stds:
    - 0.0011
  - model: TranS + NodePiece
    model_plain: TranS + NodePiece
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.215402
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6882
    metric_stds:
    - 0.0019
  - model: TripleREv3 + NodePiece
    model_plain: TripleREv3 + NodePiece
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 36.421802
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6866
    metric_stds:
    - 0.0014
  - model: InterHT + NodePiece
    model_plain: InterHT + NodePiece
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6779
    metric_stds:
    - 0.0018
  - model: A*Net
    model_plain: A*Net
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.04798'
    title: 'A*Net: A Scalable Path-based Reasoning Approach for Knowledge Graphs'
    date: Jun 7, 2022
    date_iso: '2022-06-07'
    date_display: Jun 2022
    codebase_url: https://github.com/DeepGraphLearning/AStarNet
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6767
    metric_stds:
    - null
  - model: TripleRE + NodePiece
    model_plain: TripleRE + NodePiece
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7.3
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6582
    metric_stds:
    - 0.002
  - model: TripleREv2 + NodePiece
    model_plain: TripleREv2 + NodePiece
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7.289002
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6582
    metric_stds:
    - 0.002
  - model: Qwen3-8B
    model_plain: Qwen3-8B
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.651
    metric_stds:
    - null
  - model: Qwen2.5-7B
    model_plain: Qwen2.5-7B
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.648
    metric_stds:
    - null
  - model: ComplEx-RP (50dim)
    model_plain: ComplEx-RP (50dim)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6392
    metric_stds:
    - 0.0045
  - model: ComplEx-RP
    model_plain: ComplEx-RP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 250.1674
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6392
    metric_stds:
    - 0.0045
  - model: ComplEx+RP
    model_plain: ComplEx+RP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.04798'
    title: 'A*Net: A Scalable Path-based Reasoning Approach for Knowledge Graphs'
    date: Jun 7, 2022
    date_iso: '2022-06-07'
    date_display: Jun 2022
    codebase_url: https://github.com/DeepGraphLearning/AStarNet
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6392
    metric_stds:
    - null
  - model: Information-Flow (IF) framework
    model_plain: Information-Flow (IF) framework
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2412.03783'
    title: 'Expressivity of Representation Learning on Continuous-Time Dynamic Graphs:
      An Information-Flow Centric Review'
    date: Dec 5, 2024
    date_iso: '2024-12-05'
    date_display: Dec 2024
    codebase_url: https://github.com/king/ctdg-info-flow
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.611
    metric_stds:
    - 0.011
  - model: Qwen3-1.7B
    model_plain: Qwen3-1.7B
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.607
    metric_stds:
    - null
  - model: TripleREv2
    model_plain: TripleREv2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.763337
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6045
    metric_stds:
    - 0.0017
  - model: Mistral-7B-v0.3
    model_plain: Mistral-7B-v0.3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.604
    metric_stds:
    - null
  - model: Llama3-8B
    model_plain: Llama3-8B
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.604
    metric_stds:
    - null
  - model: EdgeBank
    model_plain: EdgeBank
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6
    metric_stds:
    - null
  - model: PairRE+LRE
    model_plain: PairRE+LRE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 501.0
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2204.13957'
    title: 'PIE: a Parameter and Inference Efficient Solution for Large Scale Knowledge
      Graph Embedding Reasoning'
    date: Apr 29, 2022
    date_iso: '2022-04-29'
    date_display: Apr 2022
    codebase_url: https://github.com/migalkin/NodePiece
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.597
    metric_stds:
    - null
  - model: PairRE
    model_plain: PairRE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.3
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2204.13957'
    title: 'PIE: a Parameter and Inference Efficient Solution for Large Scale Knowledge
      Graph Embedding Reasoning'
    date: Apr 29, 2022
    date_iso: '2022-04-29'
    date_display: Apr 2022
    codebase_url: https://github.com/migalkin/NodePiece
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5805
    metric_stds:
    - null
  - model: TripleRE
    model_plain: TripleRE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 501.0
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5794
    metric_stds:
    - 0.002
  - model: TGN
    model_plain: TGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.03783'
    title: 'Expressivity of Representation Learning on Continuous-Time Dynamic Graphs:
      An Information-Flow Centric Review'
    date: Dec 5, 2024
    date_iso: '2024-12-05'
    date_display: Dec 2024
    codebase_url: https://github.com/king/ctdg-info-flow
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.577
    metric_stds:
    - 0.015
  - model: NodePiece + AutoSF
    model_plain: NodePiece + AutoSF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.8606
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2209.08271'
    title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
    date: Sep 17, 2022
    date_iso: '2022-09-17'
    date_display: Sep 2022
    codebase_url: https://github.com/DeepGraphLearning/KnowledgeGraph-
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5703
    metric_stds:
    - 0.0035
  - model: AutoSF + NodePiece
    model_plain: AutoSF + NodePiece
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.9
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5703
    metric_stds:
    - 0.0035
  - model: AutoSF
    model_plain: AutoSF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.0
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5458
    metric_stds:
    - 0.0052
  - model: PairRE
    model_plain: PairRE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2011.03798'
    title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    date: Nov 7, 2020
    date_iso: '2020-11-07'
    date_display: Nov 2020
    codebase_url: https://github.com/alipay/KnowledgeGraphEmbeddingsViaPairedRelationVectors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5289
    metric_stds:
    - 0.003
  - model: PairRE (200dim)
    model_plain: PairRE (200dim)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5208
    metric_stds:
    - 0.0027
  - model: PairRE
    model_plain: PairRE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.3348
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5208
    metric_stds:
    - 0.0027
  - model: ComplEx (250dim)
    model_plain: ComplEx (250dim)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5027
    metric_stds:
    - 0.0027
  - model: ComplEx
    model_plain: ComplEx
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1250.5695
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5027
    metric_stds:
    - 0.0027
  - model: HTGN (UTG)
    model_plain: HTGN (UTG)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.464
    metric_stds:
    - 0.005
  - model: TransE
    model_plain: TransE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.03798'
    title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    date: Nov 7, 2020
    date_iso: '2020-11-07'
    date_display: Nov 2020
    codebase_url: https://github.com/alipay/KnowledgeGraphEmbeddingsViaPairedRelationVectors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4536
    metric_stds:
    - 0.003
  - model: RotatE (250dim)
    model_plain: RotatE (250dim)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4332
    metric_stds:
    - 0.0025
  - model: RotatE
    model_plain: RotatE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.03798'
    title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    date: Nov 7, 2020
    date_iso: '2020-11-07'
    date_display: Nov 2020
    codebase_url: https://github.com/alipay/KnowledgeGraphEmbeddingsViaPairedRelationVectors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4332
    metric_stds:
    - 0.0025
  - model: RotatE (5×dim)
    model_plain: RotatE (5×dim)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2005.00687'
    title: OGB
    date: May 2, 2020
    date_iso: '2020-05-02'
    date_display: May 2020
    codebase_url: https://github.com/snap-stanford/ogb
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4332
    metric_stds:
    - 0.0025
  - model: TransE (500dim)
    model_plain: TransE (500dim)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_iso: '2022-02-10'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4256
    metric_stds:
    - 0.003
  - model: TransE
    model_plain: TransE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1250.5695
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_iso: '2022-05-27'
    date_display: May 2022
    codebase_url: https://github.com/hzli-ucas/StarGraph
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4256
    metric_stds:
    - 0.003
  - model: TransE (5×dim)
    model_plain: TransE (5×dim)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2005.00687'
    title: OGB
    date: May 2, 2020
    date_iso: '2020-05-02'
    date_display: May 2020
    codebase_url: https://github.com/snap-stanford/ogb
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4256
    metric_stds:
    - 0.003
  - model: GPT-4.1-mini
    model_plain: GPT-4.1-mini
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.425
    metric_stds:
    - null
  - model: ComplEx
    model_plain: ComplEx
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.03798'
    title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    date: Nov 7, 2020
    date_iso: '2020-11-07'
    date_display: Nov 2020
    codebase_url: https://github.com/alipay/KnowledgeGraphEmbeddingsViaPairedRelationVectors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4028
    metric_stds:
    - 0.003
  - model: ComplEx (5×dim)
    model_plain: ComplEx (5×dim)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2005.00687'
    title: OGB
    date: May 2, 2020
    date_iso: '2020-05-02'
    date_display: May 2020
    codebase_url: https://github.com/snap-stanford/ogb
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4027
    metric_stds:
    - 0.0027
  - model: TGN
    model_plain: TGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: true
    metric_values:
    - 0.396
    metric_stds:
    - 0.06
  - model: GCLSTM (UTG)
    model_plain: GCLSTM (UTG)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.374
    metric_stds:
    - 0.01
  - model: DistMult
    model_plain: DistMult
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.03798'
    title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    date: Nov 7, 2020
    date_iso: '2020-11-07'
    date_display: Nov 2020
    codebase_url: https://github.com/alipay/KnowledgeGraphEmbeddingsViaPairedRelationVectors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3729
    metric_stds:
    - 0.0045
  - model: DistMult (5×dim)
    model_plain: DistMult (5×dim)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2005.00687'
    title: OGB
    date: May 2, 2020
    date_iso: '2020-05-02'
    date_display: May 2020
    codebase_url: https://github.com/snap-stanford/ogb
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3729
    metric_stds:
    - 0.0045
  - model: GCN (UTG)
    model_plain: GCN (UTG)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.05393'
    title: Are Large Language Models Good Temporal Graph Learners?
    date: Jun 3, 2025
    date_iso: '2025-06-03'
    date_display: Jun 2025
    codebase_url: https://github.com/shenyangHuang/TGTalker
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.336
    metric_stds:
    - 0.009
  row_count: 54
  rows_json: /data/datasets/ogbl-wikikg2/standard-split-rows.json
  chart_json: /data/datasets/ogbl-wikikg2/standard-split-chart.json
  arch_counts:
    gnn: 21
    hybrid: 2
    graph_transformer: 0
    llm: 2
    walk: 0
    traditional: 19
  metric_counts:
  - 54
  milestones: &id001
  - value: 0.4332
    std: 0.0025
    model: RotatE (5×dim)
    arxiv_id: '2005.00687'
    title: OGB
    date: '2020-05-02'
  - value: 0.5289
    std: 0.003
    model: PairRE
    arxiv_id: '2011.03798'
    title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    date: '2020-11-07'
  - value: 0.7293
    std: 0.0018
    model: InterHT + DigPiece
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: '2022-02-10'
  milestones_by_metric:
    MRR: *id001
---

