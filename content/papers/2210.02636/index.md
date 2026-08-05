---
title: Geodesic Graph Neural Network for Efficient Graph Representation Learning
arxiv_id: '2210.02636'
source_url: ''
authors:
- name: Lecheng Kong
  orcid: null
  s2_author_id: '2164063663'
  s2_url: null
- name: Yixin Chen
  orcid: null
  s2_author_id: '2116664181'
  s2_url: null
- name: Muhan Zhang
  orcid: null
  s2_author_id: '1390814008'
  s2_url: null
published_date: Oct 6, 2022
published_date_iso: '2022-10-06'
published_venue: NeurIPS 2022
published_conference: NeurIPS 2022
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Graph Neural Networks (GNNs) have recently been applied to graph learning
  tasks and achieved state-of-the-art (SOTA) results. However, many competitive methods
  run GNNs multiple times with subgraph extraction and customized labeling to capture
  information that is hard for normal GNNs to learn. Such operations are time-consuming
  and do not scale to large graphs. In this paper, we propose an efficient GNN framework
  called Geodesic GNN (GDGNN) that requires only one GNN run and injects conditional
  relationships between nodes into the model without labeling. This strategy effectively
  reduces the runtime of subgraph methods. Specifically, we view the shortest paths
  between two nodes as the spatial graph context of the neighborhood around them.
  The GNN embeddings of nodes on the shortest paths are used to generate geodesic
  representations. Conditioned on the geodesic representations, GDGNN can generate
  node, link, and graph representations that carry much richer structural information
  than plain GNNs. We theoretically prove that GDGNN is more powerful than plain GNNs.
  We present experimental results to show that GDGNN achieves highly competitive performance
  with SOTA GNN models on various graph learning tasks while taking significantly
  less time.
codebase_url: https://github.com/woodcutter1998/gdgnn
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GDGNN-Vert
- GDGNN-Hor
- GDGNN-Vert-Deg
- 2-GDGNN
- 3-GDGNN
- 4-GDGNN
mrr: 0.0384
adjusted_mrr: 0.0256
mrr_dataset_count: 2
benchmark_categories:
- TU Dortmund
- OGB
- GNNBenchmark
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 3
  total: 16
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
task_categories:
- graph_classification
- link_prediction
experiment_scopes:
- edge-level
- graph-level
results:
- &id006
  dataset: CSL
  rows:
  - model: 4-GDGNN
    model_key: 4-gdgnn
    model_plain: 4-GDGNN
    value: 1.0
    std: null
    paper_value: 1.0
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Synthetic results on CSL dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0
    true_std: null
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0
    sort_std: null
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PF-GNN
    model_key: pf-gnn
    model_plain: PF-GNN
    value: 1.0
    std: null
    paper_value: 1.0
    paper_std: null
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Synthetic results on CSL dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0
    true_std: null
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0
    sort_std: null
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: ppgn
    model_plain: GPM
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
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
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: rw-agentnet
    model_plain: GPM
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
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
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: agentnet
    model_plain: GPM
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
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
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.1
    std: null
    paper_value: 0.1
    paper_std: null
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Synthetic results on CSL dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.1
    at_pub_std: 0.0
    at_pub_source_arxiv: '1905.12560'
    at_pub_source_title: On the Equivalence between Graph Isomorphism Testing and
      Function Approximation with GNNs
    at_pub_source_date_iso: '2019-05-29'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2023-01-01'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.99333
    true_std: 0.01333
    value_gap_source_arxiv: '2003.00982'
    value_gap_source_title: GNNBenchmark
    value_gap_source_is_current_paper: false
    value_gap: 0.8933300000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.99333
    sort_std: 0.01333
    global_rank: 42
    paper_rank: 79
    rank_delta: 37
    rank_delta_abs: 37
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: 3-GDGNN
    model_key: 3-gdgnn
    model_plain: 3-GDGNN
    value: 0.6
    std: null
    paper_value: 0.6
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Synthetic results on CSL dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6
    true_std: null
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6
    sort_std: null
    global_rank: 61
    paper_rank: 61
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 2-GDGNN
    model_key: 2-gdgnn
    model_plain: 2-GDGNN
    value: 0.3
    std: null
    paper_value: 0.3
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Synthetic results on CSL dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3
    true_std: null
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3
    sort_std: null
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
  - model: RNI
    model_key: rni
    model_plain: RNI
    value: 0.16
    std: null
    paper_value: 0.16
    paper_std: null
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Synthetic results on CSL dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-29'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.16
    true_std: null
    value_gap_source_arxiv: '2310.19142'
    value_gap_source_title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural
      Network'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.16
    sort_std: null
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: D&D
  rows:
  - model: ECC
    model_key: gc-gnn (graphsage)
    model_plain: ECC
    value: 0.921
    std: 0.081
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.00738'
    title: Rethinking the Power of Graph Canonization in Graph Representation Learning
      with Stability
    date: Sep 1, 2023
    date_display: Sep 2023
    date_iso: '2023-09-01'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.921
    sort_std: 0.081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: sugar
    model_plain: ECC
    value: 0.8403
    std: 0.0133
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2101.08170'
    title: 'SUGAR: Subgraph Neural Network with Reinforcement Pooling and Self-Supervised
      Mutual Information Mechanism'
    date: Jan 20, 2021
    date_display: Jan 2021
    date_iso: '2021-01-20'
    venue: The Web Conference
    codebase_url: https://github.com/RingBDStack/SUGAR
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8403
    sort_std: 0.0133
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: ortho-g-u-nets
    model_plain: ECC
    value: 0.8387
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2109.11338'
    title: Orthogonal Graph Neural Networks
    date: Sep 23, 2021
    date_display: Sep 2021
    date_iso: '2021-09-23'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8387
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.716
    std: 0.028
    paper_value: 0.716
    paper_std: 0.028
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.7912
    at_pub_std: 0.0307
    at_pub_source_arxiv: '2012.08734'
    at_pub_source_title: Hierarchical Graph Capsule Network
    at_pub_source_date_iso: '2020-12-16'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-12-16'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.07520000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7912
    true_std: 0.0307
    value_gap_source_arxiv: '2012.08734'
    value_gap_source_title: Hierarchical Graph Capsule Network
    value_gap_source_is_current_paper: false
    value_gap: 0.07520000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7912
    sort_std: 0.0307
    global_rank: 48
    paper_rank: 170
    rank_delta: 122
    rank_delta_abs: 122
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Capsule Network
    comparison_source_arxiv: '2012.08734'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.716
    std: 0.03
    paper_value: 0.716
    paper_std: 0.03
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.7805
    at_pub_std: 0.0189
    at_pub_source_arxiv: '2010.00238'
    at_pub_source_title: Multi-grained Semantics-aware Graph Neural Networks
    at_pub_source_date_iso: '2020-10-01'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-10-01'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.0645
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7805
    true_std: 0.0189
    value_gap_source_arxiv: '2010.00238'
    value_gap_source_title: Multi-grained Semantics-aware Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0645
    has_value_note: false
    value_note: ''
    sort_value: 0.7805
    sort_std: 0.0189
    global_rank: 81
    paper_rank: 170
    rank_delta: 89
    rank_delta_abs: 89
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-grained Semantics-aware Graph Neural Networks
    comparison_source_arxiv: '2010.00238'
    is_best: false
    is_std_outlier: false
  - model: Nested-GIN
    model_key: nested-gin
    model_plain: Nested-GIN
    value: 0.778
    std: 0.039
    paper_value: 0.778
    paper_std: 0.039
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.778
    true_std: 0.039
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.039
    global_rank: 87
    paper_rank: 87
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDGIN
    model_key: gdgin
    model_plain: GDGIN
    value: 0.778
    std: 0.036
    paper_value: 0.778
    paper_std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.778
    true_std: 0.036
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.036
    global_rank: 88
    paper_rank: 88
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDGCN
    model_key: gdgcn
    model_plain: GDGCN
    value: 0.776
    std: 0.04
    paper_value: 0.776
    paper_std: 0.04
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.776
    true_std: 0.04
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.776
    sort_std: 0.04
    global_rank: 95
    paper_rank: 95
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Nested-GCN
    model_key: nested-gcn
    model_plain: Nested-GCN
    value: 0.763
    std: 0.038
    paper_value: 0.763
    paper_std: 0.038
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.763
    true_std: 0.038
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.763
    sort_std: 0.038
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: MUTAG
  rows:
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
    value: 0.991
    std: 0.003
    metric: Accuracy
    higher_is_better: true
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
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: supcosine
    model_plain: ECC
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: cauemo
    model_plain: ECC
    value: 0.9692
    std: 0.0136
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.06283'
    title: 'Soft causal learning for generalized molecule property prediction: An
      environment modeling perspective'
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9692
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.74
    std: 0.088
    paper_value: 0.74
    paper_std: 0.088
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.933
    at_pub_std: 0.029
    at_pub_source_arxiv: '2112.00911'
    at_pub_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    at_pub_source_date_iso: '2021-12-02'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-12-02'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.19300000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.933
    true_std: 0.029
    value_gap_source_arxiv: '2112.00911'
    value_gap_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.19300000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.029
    global_rank: 34
    paper_rank: 730
    rank_delta: 696
    rank_delta_abs: 696
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    comparison_source_arxiv: '2112.00911'
    is_best: false
    is_std_outlier: false
  - model: GDGIN
    model_key: gdgin
    model_plain: GDGIN
    value: 0.894
    std: 0.071
    paper_value: 0.894
    paper_std: 0.071
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.894
    true_std: 0.071
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: 0.071
    global_rank: 230
    paper_rank: 230
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.734
    std: 0.108
    paper_value: 0.734
    paper_std: 0.108
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.891
    at_pub_std: 0.0581
    at_pub_source_arxiv: '2106.04319'
    at_pub_source_title: Breaking the Limits of Message Passing Graph Neural Networks
    at_pub_source_date_iso: '2021-06-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-08-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.15700000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.891
    true_std: 0.058
    value_gap_source_arxiv: '2308.08235'
    value_gap_source_title: 'The Expressive Power of Graph Neural Networks: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.15700000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.891
    sort_std: 0.058
    global_rank: 250
    paper_rank: 741
    rank_delta: 491
    rank_delta_abs: 491
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDGCN
    model_key: gdgcn
    model_plain: GDGCN
    value: 0.884
    std: 0.066
    paper_value: 0.884
    paper_std: 0.066
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.884
    true_std: 0.066
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.884
    sort_std: 0.066
    global_rank: 293
    paper_rank: 293
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Nested-GIN
    model_key: nested-gin
    model_plain: Nested-GIN
    value: 0.879
    std: 0.082
    paper_value: 0.879
    paper_std: 0.082
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.879
    true_std: 0.082
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.879
    sort_std: 0.082
    global_rank: 316
    paper_rank: 316
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Nested-GCN
    model_key: nested-gcn
    model_plain: Nested-GCN
    value: 0.829
    std: 0.111
    paper_value: 0.829
    paper_std: 0.111
    metric: Accuracy
    higher_is_better: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph classification on TU benchmark
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.829
    true_std: 0.111
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: 0.111
    global_rank: 528
    paper_rank: 528
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: ogbg-molhiv
  rows:
  - model: SigGate-GT
    model_key: multi-rf fusion with multi-gnn blending
    model_plain: SigGate-GT
    value: 0.8476
    std: 0.0002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: mixed
    feature_source_evidence: Mixing pharmacophoric (FCFP) and structural (ECFP) fingerprints...
      GNNs contributing only 12%
    is_global_top: true
    global_rank: 1
    sort_value: 0.8476
    sort_std: 0.0002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: hyperfusion
    model_plain: SigGate-GT
    value: 0.8475
    std: 0.0003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8475
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: pas+fps
    model_plain: SigGate-GT
    value: 0.842
    std: 0.0015
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.842
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGSN
    model_key: dgsn
    model_plain: DGSN
    value: 0.8039
    std: 0.009
    paper_value: 0.8039
    paper_std: 0.009
    metric: ROC-AUC
    higher_is_better: true
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on OGBG-MOLHIV
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8039
    true_std: 0.009
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8039
    sort_std: 0.009
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PF-GNN
    model_key: pf-gnn
    model_plain: PF-GNN
    value: 0.8015
    std: 0.0068
    paper_value: 0.8015
    paper_std: 0.0068
    metric: ROC-AUC
    higher_is_better: true
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on OGBG-MOLHIV
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-29'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8015
    true_std: 0.0068
    value_gap_source_arxiv: '2310.19142'
    value_gap_source_title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural
      Network'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8015
    sort_std: 0.0068
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
  - model: GIN-AK+
    model_key: gin-ak+
    model_plain: GIN-AK+
    value: 0.7822
    std: 0.0075
    paper_value: 0.7822
    paper_std: 0.0075
    metric: ROC-AUC
    higher_is_better: true
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on OGBG-MOLHIV
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7961
    true_std: 0.011
    value_gap_source_arxiv: '2312.08671'
    value_gap_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    value_gap_source_is_current_paper: false
    value_gap: 0.013900000000000023
    has_value_note: false
    value_note: ''
    sort_value: 0.7961
    sort_std: 0.011
    global_rank: 44
    paper_rank: 97
    rank_delta: 53
    rank_delta_abs: 53
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDGIN
    model_key: gdgin
    model_plain: GDGIN
    value: 0.7907
    std: 0.012
    paper_value: 0.7907
    paper_std: 0.012
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on OGBG-MOLHIV
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7907
    true_std: 0.012
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7907
    sort_std: 0.012
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Nested-GIN
    model_key: nested-gin
    model_plain: Nested-GIN
    value: 0.7834
    std: 0.0186
    paper_value: 0.7834
    paper_std: 0.0186
    metric: ROC-AUC
    higher_is_better: true
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on OGBG-MOLHIV
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7834
    true_std: 0.0186
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7834
    sort_std: 0.0186
    global_rank: 94
    paper_rank: 94
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
    value: 0.7558
    std: 0.014
    paper_value: 0.7558
    paper_std: 0.014
    metric: ROC-AUC
    higher_is_better: true
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on OGBG-MOLHIV
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.778
    at_pub_std: 0.0182
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.022199999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.778
    true_std: 0.0182
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.022199999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.0182
    global_rank: 120
    paper_rank: 237
    rank_delta: 117
    rank_delta_abs: 117
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: ogbl-collab
  rows:
  - model: SIGN
    model_key: proxi
    model_plain: SIGN
    value: 0.765
    std: 0.0027
    metric: Hits@50
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/workrep20232/PROXI
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.765
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SIGN
    model_key: ogb leader
    model_plain: SIGN
    value: 0.7129
    std: 0.0018
    metric: Hits@50
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/workrep20232/PROXI
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7129
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: gidn
    model_plain: SIGN
    value: 0.7096
    std: 0.0055
    metric: Hits@50
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.01301'
    title: 'GIDN: A Lightweight Graph Inception Diffusion Network for High-efficient
      Link Prediction'
    date: Oct 4, 2022
    date_display: Oct 2022
    date_iso: '2022-10-04'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7096
    sort_std: 0.0055
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.4475
    std: 0.0145
    paper_value: 0.4475
    paper_std: 0.0145
    metric: Hits@50
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.4714
    at_pub_std: 0.0145
    at_pub_source_arxiv: '2005.00687'
    at_pub_source_title: OGB
    at_pub_source_date_iso: '2020-05-02'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-09-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.023899999999999977
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6621
    true_std: 0.0033
    value_gap_source_arxiv: '2409.17475'
    value_gap_source_title: On the Impact of Feature Heterophily on Link Prediction
      with Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2146
    has_value_note: false
    value_note: ''
    sort_value: 0.6621
    sort_std: 0.0033
    global_rank: 7
    paper_rank: 75
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SEAL
    model_key: seal
    model_plain: SEAL
    value: 0.5437
    std: 0.0049
    paper_value: 0.5437
    paper_std: 0.0049
    metric: Hits@50
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.6474
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.10370000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6474
    true_std: 0.0043
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.10370000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.6474
    sort_std: 0.0043
    global_rank: 15
    paper_rank: 32
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: GDGNN-Vert
    model_key: gdgnn-vert
    model_plain: GDGNN-Vert
    value: 0.5474
    std: 0.0048
    paper_value: 0.5474
    paper_std: 0.0048
    metric: Hits@50
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5474
    true_std: 0.0048
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5474
    sort_std: 0.0048
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
  - model: GDGNN-Hor
    model_key: gdgnn-hor
    model_plain: GDGNN-Hor
    value: 0.5452
    std: 0.0072
    paper_value: 0.5452
    paper_std: 0.0072
    metric: Hits@50
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5452
    true_std: 0.0072
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5452
    sort_std: 0.0072
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeeperGCN
    model_key: deepergcn
    model_plain: DeeperGCN
    value: 0.5273
    std: 0.0047
    paper_value: 0.5273
    paper_std: 0.0047
    metric: Hits@50
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.5273
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2201.07858'
    at_pub_source_title: Decoupling the Depth and Scope of Graph Neural Networks
    at_pub_source_date_iso: '2022-01-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5273
    true_std: 0.0047
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5273
    sort_std: 0.0047
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.5037
    std: 0.0034
    paper_value: 0.5037
    paper_std: 0.0034
    metric: Hits@50
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.504
    at_pub_std: 0.003
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.504
    true_std: 0.003
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.504
    sort_std: 0.003
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Hits@50
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: Hits@50
  paper_metrics:
  - Hits@50
  metric: Hits@50
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: ogbl-ppa
  rows:
  - model: Classification
    model_key: mplp
    model_plain: Classification
    value: 0.6524
    std: 0.015
    metric: Hits@100
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.00976'
    title: Pure Message Passing Can Estimate Common Neighbor for Link Prediction
    date: Sep 2, 2023
    date_display: Sep 2023
    date_iso: '2023-09-02'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/Barcavin/efficient-node-labelling
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.6524
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Classification
    model_key: ogb leader
    model_plain: Classification
    value: 0.6524
    std: 0.015
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/workrep20232/PROXI
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6524
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Classification
    model_key: prb
    model_plain: Classification
    value: 0.6347
    std: 0.0175
    metric: Hits@100
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.01410'
    title: PageRank Bandits for Link Prediction
    date: Nov 3, 2024
    date_display: Nov 2024
    date_iso: '2024-11-03'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/jiaruzouu/PRB
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6347
    sort_std: 0.0175
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RA
    model_key: ra
    model_plain: RA
    value: 0.4933
    std: 0.0
    paper_value: 0.4933
    paper_std: 0.0
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.5324
    at_pub_std: 0.0
    at_pub_source_arxiv: '2112.02936'
    at_pub_source_title: Pairwise Learning for Neural Link Prediction
    at_pub_source_date_iso: '2021-12-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.03909999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5324
    true_std: 0.0
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.03909999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.5324
    sort_std: 0.0
    global_rank: 8
    paper_rank: 16
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Pairwise Learning for Neural Link Prediction
    comparison_source_arxiv: '2112.02936'
    is_best: false
    is_std_outlier: false
  - model: SEAL
    model_key: seal
    model_plain: SEAL
    value: 0.488
    std: 0.0316
    paper_value: 0.488
    paper_std: 0.0316
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.488
    at_pub_std: 0.0316
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.488
    true_std: 0.0316
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.488
    sort_std: 0.0316
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDGNN-Vert
    model_key: gdgnn-vert
    model_plain: GDGNN-Vert
    value: 0.4592
    std: 0.0214
    paper_value: 0.4592
    paper_std: 0.0214
    metric: Hits@100
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4592
    true_std: 0.0214
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4592
    sort_std: 0.0214
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDGNN-Vert-Deg
    model_key: gdgnn-vert-deg
    model_plain: GDGNN-Vert-Deg
    value: 0.4592
    std: null
    paper_value: 0.4592
    paper_std: null
    metric: Hits@100
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Ablation study on link prediction datasets
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4592
    true_std: null
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4592
    sort_std: null
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.1867
    std: 0.0132
    paper_value: 0.1867
    paper_std: 0.0132
    metric: Hits@100
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.187
    at_pub_std: 0.013
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-01'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.0002999999999999947
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2957
    true_std: 0.029
    value_gap_source_arxiv: '2310.00793'
    value_gap_source_title: 'Revisiting Link Prediction: a data perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.10900000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.2957
    sort_std: 0.029
    global_rank: 41
    paper_rank: 55
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.2888
    std: 0.0163
    paper_value: 0.2888
    paper_std: 0.0163
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.289
    at_pub_std: 0.015
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.289
    true_std: 0.015
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.289
    sort_std: 0.015
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDGNN-Hor
    model_key: gdgnn-hor
    model_plain: GDGNN-Hor
    value: 0.2879
    std: 0.038
    paper_value: 0.2879
    paper_std: 0.038
    metric: Hits@100
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on OGB dataset
    date: Oct 6, 2022
    date_display: Oct 2022
    date_iso: '2022-10-06'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-06'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2879
    true_std: 0.038
    value_gap_source_arxiv: '2210.02636'
    value_gap_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2879
    sort_std: 0.038
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
  rank_metric: Hits@100
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: Hits@100
  paper_metrics:
  - Hits@100
  metric: Hits@100
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
- benchmark: OGB
  datasets:
  - *id003
  - *id004
  - *id005
- benchmark: GNNBenchmark
  datasets:
  - *id006
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: D&D
      dataset_slug: d-d
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CSL
      dataset_slug: csl
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbl-collab
      dataset_slug: ogbl-collab
    - dataset: ogbl-ppa
      dataset_slug: ogbl-ppa
main_figure: /figures/2210.02636/main_figure.jpegoptim.jpg
---

