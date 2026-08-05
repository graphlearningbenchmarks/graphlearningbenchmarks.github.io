---
title: E(n) Equivariant Message Passing Cellular Networks
arxiv_id: '2406.03145'
source_url: ''
authors:
- name: Veljko Kovavc
  orcid: null
  s2_author_id: '2304905137'
  s2_url: null
- name: Erik J. Bekkers
  orcid: null
  s2_author_id: '2261388326'
  s2_url: null
- name: Pietro Lio
  orcid: null
  s2_author_id: '2382926836'
  s2_url: null
- name: Floor Eijkelboom
  orcid: null
  s2_author_id: '2208907804'
  s2_url: null
published_date: Jun 5, 2024
published_date_iso: '2024-06-05'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'This paper introduces E(n) Equivariant Message Passing Cellular Networks
  (EMPCNs), an extension of E(n) Equivariant Graph Neural Networks to CW-complexes.
  Our approach addresses two aspects of geometric message passing networks: 1) enhancing
  their expressiveness by incorporating arbitrary cells, and 2) achieving this in
  a computationally efficient way with a decoupled EMPCNs technique. We demonstrate
  that EMPCNs achieve close to state-of-the-art performance on multiple tasks without
  the need for steerability, including many-body predictions and motion capture. Moreover,
  ablation studies confirm that decoupled EMPCNs exhibit stronger generalization capabilities
  than their non-topologically informed counterparts. These findings show that EMPCNs
  can be used as a scalable and expressive framework for higher-order message passing
  in geometric and topological graphs'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Decoupled EMPCN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Quantum Chemistry
benchmark_coverage:
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 1
  total: 3
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: QM9
  is_multi_metric: true
  rows:
  - model: Graphormer-SPIS
    model_key: pf-gnn
    model_plain: Graphormer-SPIS
    metric_values:
    - 0.017
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    published_venue: ''
    date: Jan 31, 2024
    date_display: Jan 2024
    date_iso: '2024-01-31'
    codebase_url: https://github.com/pfgnn/PF-GNN
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.017
    sort_std: 0.001
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    metric_values:
    - null
    - 0.043
    - 0.029
    - 6.0
    - 6.0
    - 7.0
    - 0.023
    - 24.0
    - 19.0
    - 1.21
    - 6.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.019
    sort_std: 0.001
    true_value: 0.019
    true_std: 0.001
    paper_value: 0.043
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.023999999999999997
    value_gap_source_arxiv: '2401.17752'
    value_gap_source_title: 'PF-GNN: Differentiable particle filtering based approximation
      of universal graph representations'
    value_note: ''
    at_pub_value: 0.019
    at_pub_std: 0.001
    at_pub_source_arxiv: '2401.17752'
    at_pub_source_title: 'PF-GNN: Differentiable particle filtering based approximation
      of universal graph representations'
    at_pub_source_date_iso: '2024-01-31'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-01-31'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.023999999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'PF-GNN: Differentiable particle filtering based approximation
      of universal graph representations'
    comparison_source_arxiv: '2401.17752'
    is_best: true
    is_std_outlier: false
    global_rank: 2
  - model: Graphormer-SPIS
    model_key: fgnn
    model_plain: Graphormer-SPIS
    metric_values:
    - 0.027
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    published_venue: ''
    date: Jan 31, 2024
    date_display: Jan 2024
    date_iso: '2024-01-31'
    codebase_url: https://github.com/pfgnn/PF-GNN
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.027
    sort_std: 0.001
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    metric_values:
    - null
    - 0.045
    - 0.012
    - 5.0
    - 6.0
    - 7.0
    - 0.024
    - 27.0
    - 20.0
    - 1.12
    - 5.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.045
    sort_std: null
    true_value: 0.045
    true_std: null
    paper_value: 0.045
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: 0.045
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 11
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    metric_values:
    - null
    - 0.046
    - 0.026
    - 6.0
    - 6.0
    - 8.0
    - 0.021
    - 23.0
    - 18.0
    - 1.21
    - 7.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.046
    sort_std: null
    true_value: 0.046
    true_std: null
    paper_value: 0.046
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_note: ''
    at_pub_value: 0.046
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-04-07'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 12
  - model: SEGNN
    model_key: segnn
    model_plain: SEGNN
    metric_values:
    - null
    - 0.06
    - 0.023
    - 15.0
    - 16.0
    - 15.0
    - 0.031
    - 24.0
    - 21.0
    - 1.62
    - 12.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.06
    sort_std: null
    true_value: 0.06
    true_std: null
    paper_value: 0.06
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_note: ''
    at_pub_value: 0.06
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-04-07'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 20
  - model: Decoupled EMPCN
    model_key: decoupled empcn
    model_plain: Decoupled EMPCN
    metric_values:
    - null
    - 0.063
    - 0.026
    - 11.0
    - 10.0
    - 10.0
    - 0.027
    - 27.0
    - 27.0
    - 1.51
    - 10.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.063
    sort_std: null
    true_value: 0.063
    true_std: null
    paper_value: 0.063
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2406.03145'
    value_gap_source_title: E(n) Equivariant Message Passing Cellular Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-05'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: EMPSN
    model_key: empsn
    model_plain: EMPSN
    metric_values:
    - null
    - 0.066
    - 0.023
    - 10.0
    - 9.0
    - 6.0
    - 0.024
    - 25.0
    - 25.0
    - 1.37
    - 7.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.066
    sort_std: null
    true_value: 0.066
    true_std: null
    paper_value: 0.066
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2406.03145'
    value_gap_source_title: E(n) Equivariant Message Passing Cellular Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-05'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 24
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    metric_values:
    - null
    - 0.071
    - 0.029
    - 12.0
    - 12.0
    - 12.0
    - 0.031
    - 29.0
    - 29.0
    - 1.55
    - 12.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.071
    sort_std: null
    true_value: 0.071
    true_std: null
    paper_value: 0.071
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_note: ''
    at_pub_value: 0.071
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-04-07'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 27
  - model: Cormorant
    model_key: cormorant
    model_plain: Cormorant
    metric_values:
    - null
    - 0.085
    - 0.038
    - 22.0
    - 21.0
    - 20.0
    - 0.026
    - 34.0
    - 38.0
    - 2.02
    - 21.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.085
    sort_std: null
    true_value: 0.085
    true_std: null
    paper_value: 0.085
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_note: ''
    at_pub_value: 0.085
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-04-07'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 31
  - model: NMP
    model_key: nmp
    model_plain: NMP
    metric_values:
    - null
    - 0.092
    - 0.03
    - 20.0
    - 17.0
    - 19.0
    - 0.04
    - 43.0
    - 38.0
    - 1.5
    - 20.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.092
    sort_std: null
    true_value: 0.092
    true_std: null
    paper_value: 0.092
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_note: ''
    at_pub_value: 0.092
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-04-07'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 33
  - model: SE(3)-Tr.
    model_key: se(3)-tr.
    model_plain: SE(3)-Tr.
    metric_values:
    - null
    - 0.142
    - 0.051
    - null
    - null
    - null
    - null
    - 35.0
    - 33.0
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.142
    sort_std: null
    true_value: 0.142
    true_std: null
    paper_value: 0.142
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_note: ''
    at_pub_value: 0.142
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-04-07'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 36
  - model: TFN
    model_key: tfn
    model_plain: TFN
    metric_values:
    - null
    - 0.223
    - 0.064
    - null
    - null
    - null
    - null
    - 40.0
    - 38.0
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.223
    sort_std: null
    true_value: 0.223
    true_std: null
    paper_value: 0.223
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_note: ''
    at_pub_value: 0.223
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-04-07'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 40
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    metric_values:
    - null
    - 0.235
    - 0.033
    - 19.0
    - 14.0
    - 14.0
    - 0.033
    - 41.0
    - 34.0
    - 1.7
    - 19.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.235
    sort_std: null
    true_value: 0.235
    true_std: null
    paper_value: 0.235
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: 0.235
    at_pub_std: null
    at_pub_source_arxiv: '2011.14115'
    at_pub_source_title: Fast and Uncertainty-Aware Directional Message Passing for
      Non-Equilibrium Molecules
    at_pub_source_date_iso: '2020-11-28'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 46
  - model: MPSN
    model_key: mpsn
    model_plain: MPSN
    metric_values:
    - null
    - 0.266
    - 0.101
    - 33.0
    - 32.0
    - 31.0
    - 0.122
    - 89.0
    - 77.0
    - 3.02
    - 33.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.266
    sort_std: null
    true_value: 0.266
    true_std: null
    paper_value: 0.266
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2406.03145'
    value_gap_source_title: E(n) Equivariant Message Passing Cellular Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-05'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 56
  metrics:
  - gap
  - alpha
  - mu
  - U0
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - zpve
  - U
  primary_metric: gap
  rank_metric: alpha
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: gap
  paper_metrics:
  - alpha
  - mu
  - U0
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - zpve
  - U
  metric: alpha
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Quantum Chemistry
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Quantum Chemistry
    benchmark_slug: quantum-chemistry
    datasets:
    - dataset: QM9
      dataset_slug: qm9
single_proposed_model: Decoupled EMPCN
main_figure: /figures/2406.03145/main_figure.jpegoptim.jpg
---

