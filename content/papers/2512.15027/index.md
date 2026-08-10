---
title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral Contrastive Learning
  for Graph Clustering'
arxiv_id: '2512.15027'
source_url: ''
authors:
- name: Liang Peng
  orcid: null
  s2_author_id: '2330244069'
  s2_url: null
- name: Yixuan Ye
  orcid: null
  s2_author_id: '2386500158'
  s2_url: null
- name: Cheng Liu
  orcid: null
  s2_author_id: '2274360227'
  s2_url: null
- name: Hangjun Che
  orcid: null
  s2_author_id: '2481525'
  s2_url: null
- name: Man-Fai Leung
  orcid: null
  s2_author_id: '2189587987'
  s2_url: null
- name: Si Wu
  orcid: null
  s2_author_id: '2302787231'
  s2_url: null
- name: Hau-San Wong
  orcid: null
  s2_author_id: '2293401982'
  s2_url: null
published_date: Dec 17, 2025
published_date_iso: '2025-12-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Recently, neighbor-based contrastive learning has been introduced to effectively
  exploit neighborhood information for clustering. However, these methods rely on
  the homophily assumption—that connected nodes share similar class labels and should
  therefore be close in feature space—which fails to account for the varying homophily
  levels in real-world graphs. As a result, applying contrastive learning to low-homophily
  graphs may lead to indistinguishable node representations due to unreliable neighborhood
  information, making it challenging to identify trustworthy neighborhoods with varying
  homophily levels in graph clustering. To tackle this, we introduce a novel neighborhood
  Neutral Contrastive Graph Clustering method NeuCGC that extends traditional contrastive
  learning by incorporating neutral pairs—node pairs treated as weighted positive
  pairs, rather than strictly positive or negative. These neutral pairs are dynamically
  adjusted based on the graph’s homophily level, enabling a more flexible and robust
  learning process. Leveraging neutral pairs in contrastive learning, our method incorporates
  two key components: 1) an adaptive contrastive neighborhood distribution alignment
  that adjusts based on the homophily level of the given attribute graph, ensuring
  effective alignment of neighborhood distributions, and 2) a contrastive neighborhood
  node feature consistency learning mechanism that leverages reliable neighborhood
  information from high-confidence graphs to learn robust node representations, mitigating
  the adverse effects of varying homophily levels and effectively exploiting highly
  trustworthy neighborhood information. Experimental results demonstrate the effectiveness
  and robustness of our approach, outperforming other state-of-the-art graph clustering
  methods. Our code is available at.'
codebase_url: https://github.com/THPengL/NeuCGC
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- NeuCGC
mrr: 0.0023
adjusted_mrr: 0.0008
mrr_dataset_count: 1
benchmark_categories:
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Texas
  rows:
  - model: P^2GNN
    model_key: p^2gnn
    model_plain: P^2GNN
    value: 0.9672
    std: 0.0147
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9672
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.966
    std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPF-plus
    model_key: gpf-plus
    model_plain: GPF-plus
    value: 0.9583
    std: 0.0419
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.05346'
    title: 'ProG: A Graph Prompt Learning Benchmark'
    date: Jun 8, 2024
    date_display: Jun 2024
    date_iso: '2024-06-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/sheldonresearch/ProG
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9583
    sort_std: 0.0419
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.923
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_display: Oct 2024
    date_iso: '2024-10-08'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 45
    sort_value: 0.923
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9001
    std: 0.023
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 73
    sort_value: 0.9001
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HeterGCL
    model_key: hetergcl
    model_plain: HeterGCL
    value: 0.655
    std: 0.038
    paper_value: 0.655
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
    source_ref: IJCAI'24
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.747
    at_pub_std: 0.036
    at_pub_source_arxiv: '2507.20127'
    at_pub_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    at_pub_source_date_iso: '2025-07-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-07-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.09199999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.747
    true_std: 0.036
    value_gap_source_arxiv: '2507.20127'
    value_gap_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    value_gap_source_is_current_paper: false
    value_gap: 0.09199999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.747
    sort_std: 0.036
    global_rank: 398
    paper_rank: 520
    rank_delta: 122
    rank_delta_abs: 122
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for
      Graph Message-passing'
    comparison_source_arxiv: '2507.20127'
    is_best: false
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.546
    std: 0.023
    paper_value: 0.546
    paper_std: 0.023
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
    source_ref: KDD'22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7432
    at_pub_std: 0.0456
    at_pub_source_arxiv: '2408.13471'
    at_pub_source_title: Disentangled Generative Graph Representation Learning
    at_pub_source_date_iso: '2024-08-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.19719999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7432
    true_std: 0.0456
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.19719999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7432
    sort_std: 0.0456
    global_rank: 404
    paper_rank: 664
    rank_delta: 260
    rank_delta_abs: 260
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Disentangled Generative Graph Representation Learning
    comparison_source_arxiv: '2408.13471'
    is_best: false
    is_std_outlier: false
  - model: NeuCGC
    model_key: neucgc
    model_plain: NeuCGC
    value: 0.725
    std: 0.005
    paper_value: 0.725
    paper_std: 0.005
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
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.725
    true_std: 0.005
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.725
    sort_std: 0.005
    global_rank: 441
    paper_rank: 441
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphACL
    model_key: graphacl
    model_plain: GraphACL
    value: 0.607
    std: 0.017
    paper_value: 0.607
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
    source_ref: NIPS'23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7108
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2310.18884'
    at_pub_source_title: Simple and Asymmetric Graph Contrastive Learning without
      Augmentations
    at_pub_source_date_iso: '2023-10-29'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2025-06-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.1038
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7108
    true_std: 0.0034
    value_gap_source_arxiv: '2506.19343'
    value_gap_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    value_gap_source_is_current_paper: false
    value_gap: 0.1038
    has_value_note: false
    value_note: ''
    sort_value: 0.7108
    sort_std: 0.0034
    global_rank: 458
    paper_rank: 583
    rank_delta: 125
    rank_delta_abs: 125
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple and Asymmetric Graph Contrastive Learning without
      Augmentations
    comparison_source_arxiv: '2310.18884'
    is_best: false
    is_std_outlier: false
  - model: DCRN
    model_key: dcrn
    model_plain: DCRN
    value: 0.473
    std: 0.002
    paper_value: 0.473
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
    source_ref: AAAI'22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6126
    at_pub_std: 0.0045
    at_pub_source_arxiv: '2406.15797'
    at_pub_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    at_pub_source_date_iso: '2024-06-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.13960000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6126
    true_std: 0.0045
    value_gap_source_arxiv: '2406.15797'
    value_gap_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    value_gap_source_is_current_paper: false
    value_gap: 0.13960000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.6126
    sort_std: 0.0045
    global_rank: 578
    paper_rank: 688
    rank_delta: 110
    rank_delta_abs: 110
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    comparison_source_arxiv: '2406.15797'
    is_best: false
    is_std_outlier: false
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    value: 0.517
    std: 0.017
    paper_value: 0.517
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
    source_ref: AAAI'21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.606
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2406.15797'
    at_pub_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    at_pub_source_date_iso: '2024-06-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08899999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.606
    true_std: 0.0079
    value_gap_source_arxiv: '2406.15797'
    value_gap_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    value_gap_source_is_current_paper: false
    value_gap: 0.08899999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.606
    sort_std: 0.0079
    global_rank: 585
    paper_rank: 670
    rank_delta: 85
    rank_delta_abs: 85
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    comparison_source_arxiv: '2406.15797'
    is_best: false
    is_std_outlier: false
  - model: CONVERT
    model_key: convert
    model_plain: CONVERT
    value: 0.599
    std: 0.02
    paper_value: 0.599
    paper_std: 0.02
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
    source_ref: MM'23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.599
    true_std: 0.02
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.599
    sort_std: 0.02
    global_rank: 594
    paper_rank: 594
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HSAN
    model_key: hsan
    model_plain: HSAN
    value: 0.498
    std: 0.029
    paper_value: 0.498
    paper_std: 0.029
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
    source_ref: AAAI'23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5978
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2406.15797'
    at_pub_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    at_pub_source_date_iso: '2024-06-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5978
    true_std: 0.0036
    value_gap_source_arxiv: '2406.15797'
    value_gap_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    value_gap_source_is_current_paper: false
    value_gap: 0.0998
    has_value_note: false
    value_note: ''
    sort_value: 0.5978
    sort_std: 0.0036
    global_rank: 597
    paper_rank: 677
    rank_delta: 80
    rank_delta_abs: 80
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    comparison_source_arxiv: '2406.15797'
    is_best: false
    is_std_outlier: false
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.426
    std: 0.005
    paper_value: 0.426
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
    source_ref: WWW'20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.594
    at_pub_std: 0.0171
    at_pub_source_arxiv: '2406.15797'
    at_pub_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    at_pub_source_date_iso: '2024-06-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.16799999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.594
    true_std: 0.0171
    value_gap_source_arxiv: '2406.15797'
    value_gap_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    value_gap_source_is_current_paper: false
    value_gap: 0.16799999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.594
    sort_std: 0.0171
    global_rank: 605
    paper_rank: 699
    rank_delta: 94
    rank_delta_abs: 94
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    comparison_source_arxiv: '2406.15797'
    is_best: false
    is_std_outlier: false
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    value: 0.498
    std: 0.022
    paper_value: 0.498
    paper_std: 0.022
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
    source_ref: ICLR'22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.498
    true_std: 0.022
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.498
    sort_std: 0.022
    global_rank: 678
    paper_rank: 678
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DyFSS
    model_key: dyfss
    model_plain: DyFSS
    value: 0.486
    std: 0.011
    paper_value: 0.486
    paper_std: 0.011
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
    source_ref: AAAI'24
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.486
    true_std: 0.011
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.486
    sort_std: 0.011
    global_rank: 685
    paper_rank: 685
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CCGC
    model_key: ccgc
    model_plain: CCGC
    value: 0.479
    std: 0.035
    paper_value: 0.479
    paper_std: 0.035
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
    source_ref: AAAI'23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.479
    true_std: 0.035
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.479
    sort_std: 0.035
    global_rank: 688
    paper_rank: 688
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SCGC
    model_key: scgc
    model_plain: SCGC
    value: 0.459
    std: 0.046
    paper_value: 0.459
    paper_std: 0.046
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
    source_ref: TNNLS'23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.459
    true_std: 0.046
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.459
    sort_std: 0.046
    global_rank: 693
    paper_rank: 693
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    value: 0.432
    std: 0.039
    paper_value: 0.432
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
    source_ref: IJCAI'22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.432
    true_std: 0.039
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.432
    sort_std: 0.039
    global_rank: 699
    paper_rank: 699
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCluster
    model_key: dgcluster
    model_plain: DGCluster
    value: 0.425
    std: 0.035
    paper_value: 0.425
    paper_std: 0.035
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
    source_ref: AAAI'24
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.425
    true_std: 0.035
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.425
    sort_std: 0.035
    global_rank: 701
    paper_rank: 701
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SCAGC
    model_key: scagc
    model_plain: SCAGC
    value: 0.402
    std: 0.008
    paper_value: 0.402
    paper_std: 0.008
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
    source_ref: TMM'23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.402
    true_std: 0.008
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.402
    sort_std: 0.008
    global_rank: 702
    paper_rank: 702
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NCLA
    model_key: ncla
    model_plain: NCLA
    value: 0.382
    std: 0.033
    paper_value: 0.382
    paper_std: 0.033
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
    source_ref: AAAI'23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average clustering performance under 10 runs.
    date: Dec 17, 2025
    date_display: Dec 2025
    date_iso: '2025-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.382
    true_std: 0.033
    value_gap_source_arxiv: '2512.15027'
    value_gap_source_title: 'Trustworthy Neighborhoods Mining: Homophily-Aware Neutral
      Contrastive Learning for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.382
    sort_std: 0.033
    global_rank: 705
    paper_rank: 705
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
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
single_proposed_model: NeuCGC
main_figure: /figures/2512.15027/main_figure.jpegoptim.jpg
---

