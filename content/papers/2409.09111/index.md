---
title: 'Transformers from Diffusion: A Unified Framework for Neural Message Passing'
arxiv_id: '2409.09111'
source_url: ''
authors:
- name: Qitian Wu
  orcid: null
  s2_author_id: '51171144'
  s2_url: null
- name: David Wipf
  orcid: null
  s2_author_id: '121090473'
  s2_url: null
- name: Junchi Yan
  orcid: null
  s2_author_id: '2257137866'
  s2_url: null
published_date: Sep 13, 2024
published_date_iso: '2024-09-13'
published_venue: JMLR 2024
published_conference: JMLR 2024
published_conference_short: JMLR
published_conference_slug: jmlr
abstract: Learning representations for structured data with certain geometries (e.g.,
  observed or unobserved) is a fundamental challenge, wherein message passing neural
  networks (MPNNs) have become a de facto class of model solutions. In this paper,
  inspired by physical systems, we propose an energy-constrained diffusion model,
  which integrates the inductive bias of diffusion on manifolds with layer-wise constraints
  of energy minimization. We identify that the diffusion operators have a one-to-one
  correspondence with the energy functions implicitly descended by the diffusion process,
  and the finite-difference iteration for solving the energy-constrained diffusion
  system induces the propagation layers of various types of MPNNs operating on observed
  or latent structures. This leads to a unified mathematical framework for common
  neural architectures whose computational flows can be cast as message passing (or
  its special case), including MLPs, GNNs, and Transformers. Building on these insights,
  we devise a new class of neural message passing models, dubbed diffusion-inspired
  Transformers (DIFFormer), whose global attention layers are derived from the principled
  energy-constrained diffusion framework. Across diverse datasets ranging from real-world
  networks to images, texts, and physical particles, we demonstrate that the new model
  achieves promising performance in scenarios where the data structures are observed
  (as a graph), partially observed, or entirely unobserved.
codebase_url: https://github.com/qitianwu/DIFFormer
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DIFFormer-s
- DIFFORMER-a
mrr: 0.0153
adjusted_mrr: 0.0102
mrr_dataset_count: 2
benchmark_categories:
- Classic
- LINKX Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: LINKX Benchmarks
  benchmark_slug: linkx-benchmarks
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Cora
  rows:
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.9635
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9635
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.9629
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9629
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Coral
    model_key: coral
    model_plain: Coral
    value: 0.9574
    std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9574
    sort_std: 0.0039
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.815
    std: 0.013
    paper_value: 0.815
    paper_std: 0.013
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.08540000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08540000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 42
    paper_rank: 709
    rank_delta: 667
    rank_delta_abs: 667
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8911
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 75
    sort_value: 0.8911
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.83
    std: 0.007
    paper_value: 0.83
    paper_std: 0.007
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.05900000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.059700000000000086
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: null
    global_rank: 81
    paper_rank: 551
    rank_delta: 470
    rank_delta_abs: 470
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.834
    std: 0.002
    paper_value: 0.834
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.8848
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.05080000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8848
    true_std: 0.0327
    value_gap_source_arxiv: '2602.19622'
    value_gap_source_title: 'VecFormer: Towards Efficient and Generalizable Graph
      Transformer with Graph Token Attention'
    value_gap_source_is_current_paper: false
    value_gap: 0.05080000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8848
    sort_std: 0.0327
    global_rank: 114
    paper_rank: 501
    rank_delta: 387
    rank_delta_abs: 387
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    comparison_source_arxiv: '2401.15569'
    is_best: false
    is_std_outlier: false
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: 0.833
    std: 0.013
    paper_value: 0.833
    paper_std: 0.013
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.8815
    at_pub_std: null
    at_pub_source_arxiv: '2307.16092'
    at_pub_source_title: Feature Transportation Improves Graph Neural Networks
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: 0.04849999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8815
    true_std: null
    value_gap_source_arxiv: '2307.16092'
    value_gap_source_title: Feature Transportation Improves Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.04849999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8815
    sort_std: null
    global_rank: 136
    paper_rank: 511
    rank_delta: 375
    rank_delta_abs: 375
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Transportation Improves Graph Neural Networks
    comparison_source_arxiv: '2307.16092'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.81
    std: 0.0
    paper_value: 0.81
    paper_std: 0.0
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.8683
    at_pub_std: 0.0128
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.05829999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8797
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.06969999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8797
    sort_std: null
    global_rank: 148
    paper_rank: 749
    rank_delta: 601
    rank_delta_abs: 601
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.809
    std: 0.011
    paper_value: 0.809
    paper_std: 0.011
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.8244
    at_pub_std: 0.006
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.01539999999999997
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8603
    true_std: 0.0054
    value_gap_source_arxiv: '2510.21267'
    value_gap_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0512999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8603
    sort_std: 0.0054
    global_rank: 271
    paper_rank: 757
    rank_delta: 486
    rank_delta_abs: 486
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIFFormer-s
    model_key: difformer-s
    model_plain: DIFFormer-s
    value: 0.859
    std: 0.004
    paper_value: 0.859
    paper_std: 0.004
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.859
    at_pub_std: 0.004
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.859
    true_std: 0.004
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.859
    sort_std: 0.004
    global_rank: 276
    paper_rank: 276
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRAND-l
    model_key: grand-l
    model_plain: GRAND-l
    value: 0.836
    std: 0.01
    paper_value: 0.836
    paper_std: 0.01
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.847
    at_pub_std: 0.006
    at_pub_source_arxiv: '2106.10934'
    at_pub_source_title: 'GRAND: Graph Neural Diffusion'
    at_pub_source_date_iso: '2021-06-21'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2021-06-21'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: 0.01100000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.847
    true_std: 0.006
    value_gap_source_arxiv: '2106.10934'
    value_gap_source_title: 'GRAND: Graph Neural Diffusion'
    value_gap_source_is_current_paper: false
    value_gap: 0.01100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.847
    sort_std: 0.006
    global_rank: 353
    paper_rank: 463
    rank_delta: 110
    rank_delta_abs: 110
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIFFORMER-a
    model_key: difformer-a
    model_plain: DIFFORMER-a
    value: 0.841
    std: 0.006
    paper_value: 0.841
    paper_std: 0.006
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.841
    at_pub_std: 0.006
    at_pub_source_arxiv: '2210.13148'
    at_pub_source_title: Transformers over Directed Acyclic Graphs
    at_pub_source_date_iso: '2022-10-24'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.841
    true_std: 0.006
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.841
    sort_std: 0.006
    global_rank: 404
    paper_rank: 404
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LDS
    model_key: lds
    model_plain: LDS
    value: 0.839
    std: 0.006
    paper_value: 0.839
    paper_std: 0.006
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.839
    at_pub_std: 0.006
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.839
    true_std: 0.006
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.839
    sort_std: 0.006
    global_rank: 424
    paper_rank: 424
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphHeat
    model_key: graphheat
    model_plain: GraphHeat
    value: 0.837
    std: null
    paper_value: 0.837
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.837
    at_pub_std: null
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.837
    true_std: null
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.837
    sort_std: null
    global_rank: 446
    paper_rank: 446
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDC
    model_key: gdc
    model_plain: GDC
    value: 0.836
    std: 0.002
    paper_value: 0.836
    paper_std: 0.002
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.836
    at_pub_std: 0.002
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.836
    true_std: 0.002
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.002
    global_rank: 468
    paper_rank: 468
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLCN
    model_key: glcn
    model_plain: GLCN
    value: 0.831
    std: 0.005
    paper_value: 0.831
    paper_std: 0.005
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.831
    at_pub_std: 0.005
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.831
    true_std: 0.005
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.005
    global_rank: 542
    paper_rank: 542
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.742
    std: 0.009
    paper_value: 0.742
    paper_std: 0.009
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.8041
    at_pub_std: 0.003
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.062100000000000044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8041
    true_std: 0.002
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: false
    value_gap: 0.062100000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.8041
    sort_std: 0.002
    global_rank: 772
    paper_rank: 909
    rank_delta: 137
    rank_delta_abs: 137
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Language is All a Graph Needs
    comparison_source_arxiv: '2308.07134'
    is_best: false
    is_std_outlier: false
  - model: Dense GAT
    model_key: dense gat
    model_plain: Dense GAT
    value: 0.785
    std: 0.025
    paper_value: 0.785
    paper_std: 0.025
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.785
    at_pub_std: 0.025
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.785
    true_std: 0.025
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.785
    sort_std: 0.025
    global_rank: 834
    paper_rank: 834
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.561
    std: 0.016
    paper_value: 0.561
    paper_std: 0.016
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.7768
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.2158
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2158
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 853
    paper_rank: 1026
    rank_delta: 173
    rank_delta_abs: 173
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: GAT-kNN
    model_key: gat-knn
    model_plain: GAT-kNN
    value: 0.738
    std: 0.017
    paper_value: 0.738
    paper_std: 0.017
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.738
    at_pub_std: 0.017
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.738
    true_std: 0.017
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.738
    sort_std: 0.017
    global_rank: 913
    paper_rank: 913
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN-kNN
    model_key: gcn-knn
    model_plain: GCN-kNN
    value: 0.722
    std: 0.018
    paper_value: 0.722
    paper_std: 0.018
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.722
    at_pub_std: 0.018
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.722
    true_std: 0.018
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.722
    sort_std: 0.018
    global_rank: 935
    paper_rank: 935
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LP
    model_key: lp
    model_plain: LP
    value: 0.682
    std: null
    paper_value: 0.682
    paper_std: null
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.682
    at_pub_std: null
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.71
    true_std: 0.0
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: 0.027999999999999914
    has_value_note: false
    value_note: ''
    sort_value: 0.71
    sort_std: 0.0
    global_rank: 941
    paper_rank: 966
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ManiReg
    model_key: manireg
    model_plain: ManiReg
    value: 0.604
    std: 0.008
    paper_value: 0.604
    paper_std: 0.008
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.604
    at_pub_std: 0.008
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.604
    true_std: 0.008
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.604
    sort_std: 0.008
    global_rank: 1007
    paper_rank: 1007
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: Pokec
  rows:
  - model: Polynormer-r
    model_key: polynormer-r
    model_plain: Polynormer-r
    value: 0.861
    std: 0.0005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/cornell-zhang/Polynormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.861
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.8595
    std: 0.0007
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/cornell-zhang/Polynormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8595
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoE-H2GCN
    model_key: moe-h2gcn
    model_plain: MoE-H2GCN
    value: 0.8302
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_display: Nov 2023
    date_iso: '2023-11-09'
    venue: Accepted for publication in ICLR 2024
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8302
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6231
    std: 0.0113
    paper_value: 0.6231
    paper_std: 0.0113
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing accuracy on Pokec
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.7601
    at_pub_std: 0.0049
    at_pub_source_arxiv: '2311.05185'
    at_pub_source_title: Mixture of Weak & Strong Experts on Graphs
    at_pub_source_date_iso: '2023-11-09'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-11-09'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.137
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7601
    true_std: 0.0049
    value_gap_source_arxiv: '2311.05185'
    value_gap_source_title: Mixture of Weak & Strong Experts on Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.137
    has_value_note: false
    value_note: ''
    sort_value: 0.7601
    sort_std: 0.0049
    global_rank: 26
    paper_rank: 46
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Mixture of Weak & Strong Experts on Graphs
    comparison_source_arxiv: '2311.05185'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7576
    std: 0.0004
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_display: Nov 2023
    date_iso: '2023-11-09'
    venue: Accepted for publication in ICLR 2024
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 27
    sort_value: 0.7576
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.6557
    std: 0.0034
    paper_value: 0.6557
    paper_std: 0.0034
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing accuracy on Pokec
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.7223
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.0666000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7223
    true_std: 0.0018
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.0666000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7223
    sort_std: 0.0018
    global_rank: 32
    paper_rank: 39
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.5203
    std: 0.0084
    paper_value: 0.5203
    paper_std: 0.0084
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing accuracy on Pokec
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.7124
    at_pub_std: 0.0046
    at_pub_source_arxiv: '2202.04187'
    at_pub_source_title: 'FMP: Toward Fair Graph Message Passing against Topology
      Bias'
    at_pub_source_date_iso: '2022-02-08'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-08'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.19210000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7124
    true_std: 0.0046
    value_gap_source_arxiv: '2202.04187'
    value_gap_source_title: 'FMP: Toward Fair Graph Message Passing against Topology
      Bias'
    value_gap_source_is_current_paper: false
    value_gap: 0.19210000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.7124
    sort_std: 0.0046
    global_rank: 33
    paper_rank: 50
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'FMP: Toward Fair Graph Message Passing against Topology
      Bias'
    comparison_source_arxiv: '2202.04187'
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.6832
    std: 0.0045
    paper_value: 0.6832
    paper_std: 0.0045
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing accuracy on Pokec
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.71
    at_pub_std: 0.013
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.026799999999999935
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.71
    true_std: 0.013
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.026799999999999935
    has_value_note: false
    value_note: ''
    sort_value: 0.71
    sort_std: 0.013
    global_rank: 34
    paper_rank: 37
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6015
    std: 0.0003
    paper_value: 0.6015
    paper_std: 0.0003
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing accuracy on Pokec
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.7048
    at_pub_std: 0.0077
    at_pub_source_arxiv: '2202.04187'
    at_pub_source_title: 'FMP: Toward Fair Graph Message Passing against Topology
      Bias'
    at_pub_source_date_iso: '2022-02-08'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-08'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.10329999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7048
    true_std: 0.0077
    value_gap_source_arxiv: '2202.04187'
    value_gap_source_title: 'FMP: Toward Fair Graph Message Passing against Topology
      Bias'
    value_gap_source_is_current_paper: false
    value_gap: 0.10329999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7048
    sort_std: 0.0077
    global_rank: 36
    paper_rank: 47
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'FMP: Toward Fair Graph Message Passing against Topology
      Bias'
    comparison_source_arxiv: '2202.04187'
    is_best: false
    is_std_outlier: false
  - model: DIFFormer-s
    model_key: difformer-s
    model_plain: DIFFormer-s
    value: 0.6924
    std: 0.0076
    paper_value: 0.6924
    paper_std: 0.0076
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing accuracy on Pokec
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.6924
    at_pub_std: 0.0076
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6924
    true_std: 0.0076
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6924
    sort_std: 0.0076
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LP
    model_key: lp
    model_plain: LP
    value: 0.5273
    std: null
    paper_value: 0.5273
    paper_std: null
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing accuracy on Pokec
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: JMLR 2024
    published_conference: JMLR 2024
    at_pub_value: 0.5273
    at_pub_std: null
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5273
    true_std: null
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5273
    sort_std: null
    global_rank: 50
    paper_rank: 50
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: LINKX Benchmarks
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: Pokec
      dataset_slug: pokec
main_figure: /figures/2409.09111/main_figure.jpegoptim.jpg
---

