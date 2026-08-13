---
title: WN18
slug: wn18
benchmark: Knowledge Graphs
task_type: link_prediction
short_description: Knowledge graph link prediction on WordNet (full, 18 relations).
description: '**18-relation knowledge-graph completion** Knowledge graph link prediction
  on WordNet (full, 18 relations). Inputs are directed subject-relation-object triples
  with learned embeddings. Inverse relations make this legacy split highly vulnerable
  to leakage. Evaluated by MRR.'
detailed_description:
  task: Knowledge graph link prediction on WordNet (full, 18 relations). The primary
    catalog metric is MRR.
  data: Knowledge graph link prediction on WordNet (full, 18 relations).
  features: The raw input is a set of directed subject-relation-object triples. Entity
    and relation embeddings are learned inputs; reciprocal edges, inverse relations,
    and filtered candidate sets are evaluation or preprocessing choices.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses MRR (higher is better). Exact masks or folds must come
    from the cited release.'
  quirks_and_pitfalls: Filtered ranking removes other known true triples but the graph
    is incomplete, so sampled corruptions can be false negatives. WN18 and FB15k contain
    inverse-relation leakage; use WN18RR or FB15k-237 when evaluating relational generalization.
sources:
- title: Translating Embeddings for Modeling Multi-relational Data
  arxiv_id: '1301.3485'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric WN18 loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.WordNet18.html
  kind: implementation_documentation
primary_metric: MRR
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.WordNet18.html
stats: null
result_count: 16
best_model:
  model: Inverse Model
  value: 0.963
  metric: MRR
  arxiv_id: '1707.01476'
  paper_title: Knowledge Graphs
papers:
- arxiv_id: '2209.08271'
  title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
  date_iso: '2022-09-17'
  venue: ''
- arxiv_id: '1902.10197'
  title: 'RotatE: Knowledge Graph Embedding by Relational Rotation in Complex Space'
  date_iso: '2018-09-27'
  venue: ICLR 2018
- arxiv_id: '1707.01476'
  title: Knowledge Graphs
  date_iso: '2017-07-05'
  venue: AAAI 2017
- arxiv_id: '1703.06103'
  title: Modeling Relational Data with Graph Convolutional Networks
  date_iso: '2017-03-17'
  venue: ''
- arxiv_id: '1606.06357'
  title: Complex Embeddings for Simple Link Prediction
  date_iso: '2016-06-19'
  venue: ICML 2016
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MRR
  default_metric: MRR
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - MRR
  - Hit@10
  metric_display_names:
  - MRR
  - Hit@10
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: Inverse Model
    model_plain: Inverse Model
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1707.01476'
    title: Knowledge Graphs
    date: Jul 5, 2017
    date_iso: '2017-07-05'
    date_display: Jul 2017
    codebase_url: https://github.com/TimDettmers/ConvE
    published_conference: AAAI 2017
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2017
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.963
    - null
    metric_stds:
    - null
    - null
  - model: RotatE
    model_plain: RotatE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1902.10197'
    title: 'RotatE: Knowledge Graph Embedding by Relational Rotation in Complex Space'
    date: Sep 27, 2018
    date_iso: '2018-09-27'
    date_display: Sep 2018
    codebase_url: https://github.com/DeepGraphLearning/KnowledgeGraphEmbedding
    published_conference: ICLR 2018
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2018
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.949
    - null
    metric_stds:
    - 0.0
    - null
  - model: ConvE
    model_plain: ConvE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1707.01476'
    title: Knowledge Graphs
    date: Jul 5, 2017
    date_iso: '2017-07-05'
    date_display: Jul 2017
    codebase_url: https://github.com/TimDettmers/ConvE
    published_conference: AAAI 2017
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.943
    - null
    metric_stds:
    - null
    - null
  - model: ANALOGY
    model_plain: ANALOGY
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '1707.01476'
    title: Knowledge Graphs
    date: Jul 5, 2017
    date_iso: '2017-07-05'
    date_display: Jul 2017
    codebase_url: https://github.com/TimDettmers/ConvE
    published_conference: AAAI 2017
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.942
    - null
    metric_stds:
    - null
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
    arxiv_id: '1703.06103'
    title: Modeling Relational Data with Graph Convolutional Networks
    date: Mar 17, 2017
    date_iso: '2017-03-17'
    date_display: Mar 2017
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.941
    - null
    metric_stds:
    - null
    - null
  - model: HolE
    model_plain: HolE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1606.06357'
    title: Complex Embeddings for Simple Link Prediction
    date: Jun 19, 2016
    date_iso: '2016-06-19'
    date_display: Jun 2016
    codebase_url: https://github.com/ttrouill/complex
    published_conference: ICML 2016
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.938
    - null
    metric_stds:
    - null
    - null
  - model: LinkFeat
    model_plain: LinkFeat
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1703.06103'
    title: Modeling Relational Data with Graph Convolutional Networks
    date: Mar 17, 2017
    date_iso: '2017-03-17'
    date_display: Mar 2017
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.938
    - null
    metric_stds:
    - null
    - null
  - model: DistMult
    model_plain: DistMult
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1606.06357'
    title: Complex Embeddings for Simple Link Prediction
    date: Jun 19, 2016
    date_iso: '2016-06-19'
    date_display: Jun 2016
    codebase_url: https://github.com/ttrouill/complex
    published_conference: ICML 2016
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.822
    - null
    metric_stds:
    - null
    - null
  - model: R-GCN
    model_plain: R-GCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.06103'
    title: Modeling Relational Data with Graph Convolutional Networks
    date: Mar 17, 2017
    date_iso: '2017-03-17'
    date_display: Mar 2017
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.819
    - null
    metric_stds:
    - null
    - null
  - model: R-GCN
    model_plain: R-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1707.01476'
    title: Knowledge Graphs
    date: Jul 5, 2017
    date_iso: '2017-07-05'
    date_display: Jul 2017
    codebase_url: https://github.com/TimDettmers/ConvE
    published_conference: AAAI 2017
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.814
    - null
    metric_stds:
    - null
    - null
  - model: DistMult
    model_plain: DistMult
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.06103'
    title: Modeling Relational Data with Graph Convolutional Networks
    date: Mar 17, 2017
    date_iso: '2017-03-17'
    date_display: Mar 2017
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.813
    - null
    metric_stds:
    - null
    - null
  - model: TripleRE
    model_plain: TripleRE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
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
    - 0.7725
    - 0.9541
    metric_stds:
    - null
    - null
  - model: TransAt
    model_plain: TransAt
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
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
    - 0.6446
    - 0.951
    metric_stds:
    - null
    - null
  - model: TransE
    model_plain: TransE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1606.06357'
    title: Complex Embeddings for Simple Link Prediction
    date: Jun 19, 2016
    date_iso: '2016-06-19'
    date_display: Jun 2016
    codebase_url: https://github.com/ttrouill/complex
    published_conference: ICML 2016
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.454
    - null
    metric_stds:
    - null
    - null
  - model: CP
    model_plain: CP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1606.06357'
    title: Complex Embeddings for Simple Link Prediction
    date: Jun 19, 2016
    date_iso: '2016-06-19'
    date_display: Jun 2016
    codebase_url: https://github.com/ttrouill/complex
    published_conference: ICML 2016
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.075
    - null
    metric_stds:
    - null
    - null
  - model: CP
    model_plain: CP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.06103'
    title: Modeling Relational Data with Graph Convolutional Networks
    date: Mar 17, 2017
    date_iso: '2017-03-17'
    date_display: Mar 2017
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.058
    - null
    metric_stds:
    - null
    - null
  row_count: 16
  rows_json: ''
  chart_json: /data/datasets/wn18/standard-split-chart.json
  arch_counts:
    gnn: 11
    hybrid: 0
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 4
  metric_counts:
  - 16
  - 2
  milestones: &id001
  - value: 0.938
    std: null
    model: HolE
    arxiv_id: '1606.06357'
    title: Complex Embeddings for Simple Link Prediction
    date: '2016-06-19'
  - value: 0.941
    std: null
    model: ComplEx
    arxiv_id: '1703.06103'
    title: Modeling Relational Data with Graph Convolutional Networks
    date: '2017-03-17'
  - value: 0.963
    std: null
    model: Inverse Model
    arxiv_id: '1707.01476'
    title: Knowledge Graphs
    date: '2017-07-05'
  milestones_by_metric:
    MRR: *id001
    Hit@10:
    - value: 0.9541
      std: null
      model: TripleRE
      arxiv_id: '2209.08271'
      title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
      date: '2022-09-17'
---

