---
title: Equivariant Spherical Transformer for Efficient Molecular Modeling
arxiv_id: '2505.23086'
source_url: ''
authors:
- name: Junyi An
  orcid: null
  s2_author_id: '2327995357'
  s2_url: null
- name: Xinyu Lu
  orcid: null
  s2_author_id: '2292660630'
  s2_url: null
- name: Chao Qu
  orcid: null
  s2_author_id: '2313621280'
  s2_url: null
- name: Yunfei Shi
  orcid: null
  s2_author_id: '2345527145'
  s2_url: null
- name: Peijia Lin
  orcid: null
  s2_author_id: '2239069738'
  s2_url: null
- name: Qianwei Tang
  orcid: null
  s2_author_id: '2346995467'
  s2_url: null
- name: Li-Cheng Xu
  orcid: null
  s2_author_id: '2377235345'
  s2_url: null
- name: Fenglei Cao
  orcid: null
  s2_author_id: '2313623018'
  s2_url: null
- name: Yuan Qi
  orcid: null
  s2_author_id: '2347889068'
  s2_url: null
published_date: May 29, 2025
published_date_iso: '2025-05-29'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Equivariant Graph Neural Networks (GNNs) have significantly advanced the
  modeling of 3D molecular structure by leveraging group representations. However,
  their message passing, heavily relying on Clebsch-Gordan tensor product convolutions,
  suffers from restricted expressiveness due to the limited non-linearity and low
  degree of group representations. To overcome this, we introduce the Equivariant
  Spherical Transformer (EST), a novel plug-and-play framework that applies a Transformer-like
  architecture to the Fourier spatial domain of group representations. EST achieves
  higher expressiveness than conventional models while preserving the crucial equivariant
  inductive bias through a uniform sampling strategy of spherical Fourier transforms.
  As demonstrated by our experiments on challenging benchmarks like OC20 and QM9,
  EST-based models achieve state-of-the-art performance. For the complex molecular
  systems within OC20, small models empowered by EST can outperform some larger models
  and those using additional data. In addition to demonstrating such strong expressiveness,we
  provide both theoretical and experimental validation of EST's equivariance as well,
  paving the way for new research in this area.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- EST (with GA)
- EST
mrr: 0.05
adjusted_mrr: 0.0167
mrr_dataset_count: 1
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
  - model: DimeNet++
    model_key: pf-gnn
    model_plain: DimeNet++
    metric_values:
    - 0.017
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
    - 33.0
    - 0.044
    - 0.03
    - 6.0
    - 7.0
    - 8.0
    - 0.023
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
    paper_value: 33.0
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 32.981
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
    gap_vs_at_pub: 32.981
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
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
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
  - model: DimeNet++
    model_key: molformer
    model_plain: DimeNet++
    metric_values:
    - 0.025
    - null
    - null
    - null
    - null
    - null
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
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    published_venue: ''
    date: Oct 4, 2021
    date_display: Oct 2021
    date_iso: '2021-10-04'
    codebase_url: https://github.com/smiles724/Molformer
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.025
    sort_std: null
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
  - model: EST (with GA)
    model_key: est (with ga)
    model_plain: EST (with GA)
    metric_values:
    - null
    - 0.041
    - null
    - null
    - null
    - null
    - 0.021
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
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.041
    sort_std: null
    true_value: 0.041
    true_std: null
    paper_value: 0.041
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2505.23086'
    value_gap_source_title: Equivariant Spherical Transformer for Efficient Molecular
      Modeling
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: '2025'
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
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    metric_values:
    - 46.0
    - 0.045
    - 0.012
    - 5.83
    - 7.35
    - 7.35
    - 0.024
    - 5.83
    metric_stds:
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
    paper_value: 46.0
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 45.954
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: 0.046
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 45.954
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
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    metric_values:
    - 63.0
    - 0.235
    - 0.033
    - 19.0
    - 14.0
    - 14.0
    - 0.033
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
    is_baseline: true
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
    paper_value: 63.0
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 62.937
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: 0.063
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 62.937
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
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 15
  - model: EST
    model_key: est
    model_plain: EST
    metric_values:
    - 28.0
    - null
    - 0.011
    - 5.92
    - 7.03
    - 7.03
    - null
    - 5.92
    metric_stds:
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
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 28.0
    sort_std: null
    true_value: 28.0
    true_std: null
    paper_value: 28.0
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2505.23086'
    value_gap_source_title: Equivariant Spherical Transformer for Efficient Molecular
      Modeling
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: '2025'
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
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
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
  - model: Equiformer v2
    model_key: equiformer v2
    model_plain: Equiformer v2
    metric_values:
    - 29.0
    - 0.05
    - 0.01
    - 6.49
    - 7.57
    - 7.57
    - 0.023
    - 6.49
    metric_stds:
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
    sort_value: 29.0
    sort_std: null
    true_value: 29.0
    true_std: null
    paper_value: 29.0
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2505.23086'
    value_gap_source_title: Equivariant Spherical Transformer for Efficient Molecular
      Modeling
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: '2025'
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
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 21
  - model: Equiformer
    model_key: equiformer
    model_plain: Equiformer
    metric_values:
    - 30.0
    - 0.046
    - 0.011
    - 6.74
    - 7.63
    - 7.63
    - 0.023
    - 6.74
    metric_stds:
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
    sort_value: 30.0
    sort_std: null
    true_value: 30.0
    true_std: null
    paper_value: 30.0
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2505.23086'
    value_gap_source_title: Equivariant Spherical Transformer for Efficient Molecular
      Modeling
    value_note: ''
    at_pub_value: 33.0
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 3.0
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    comparison_source_arxiv: '2304.04757'
    is_best: false
    is_std_outlier: false
    global_rank: 22
  - model: EQGAT
    model_key: eqgat
    model_plain: EQGAT
    metric_values:
    - 32.0
    - 0.053
    - 0.011
    - 25.0
    - 23.0
    - 23.0
    - 0.024
    - 25.0
    metric_stds:
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
    sort_value: 32.0
    sort_std: null
    true_value: 32.0
    true_std: null
    paper_value: 32.0
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2505.23086'
    value_gap_source_title: Equivariant Spherical Transformer for Efficient Molecular
      Modeling
    value_note: ''
    at_pub_value: 44.0
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 12.0
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    comparison_source_arxiv: '2304.04757'
    is_best: false
    is_std_outlier: false
    global_rank: 26
  - model: TorchMD-Net
    model_key: torchmd-net
    model_plain: TorchMD-Net
    metric_values:
    - 36.0
    - 0.059
    - 0.011
    - 6.38
    - 7.62
    - 7.62
    - 0.026
    - 6.38
    metric_stds:
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
    sort_value: 36.0
    sort_std: null
    true_value: 36.0
    true_std: null
    paper_value: 36.0
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2505.23086'
    value_gap_source_title: Equivariant Spherical Transformer for Efficient Molecular
      Modeling
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: '2025'
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
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 28
  - model: SEGNN
    model_key: segnn
    model_plain: SEGNN
    metric_values:
    - 42.0
    - 0.06
    - 0.023
    - 13.0
    - 15.0
    - 15.0
    - 0.031
    - 13.0
    metric_stds:
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
    sort_value: 42.0
    sort_std: null
    true_value: 42.0
    true_std: null
    paper_value: 42.0
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2505.23086'
    value_gap_source_title: Equivariant Spherical Transformer for Efficient Molecular
      Modeling
    value_note: ''
    at_pub_value: 42.0
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: '2025'
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
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 30
  - model: TFN
    model_key: tfn
    model_plain: TFN
    metric_values:
    - 58.0
    - 0.223
    - 0.064
    - null
    - null
    - null
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
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 58.0
    sort_std: null
    true_value: 58.0
    true_std: null
    paper_value: 58.0
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2505.23086'
    value_gap_source_title: Equivariant Spherical Transformer for Efficient Molecular
      Modeling
    value_note: ''
    at_pub_value: 58.0
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: '2025'
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
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 35
  metrics:
  - gap
  - alpha
  - mu
  - U0
  - H
  - G
  - Cv
  - U
  primary_metric: gap
  rank_metric: gap
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: gap
  paper_metrics:
  - alpha
  - gap
  - mu
  - U0
  - H
  - G
  - Cv
  - U
  metric: gap
  uses_non_primary_metric: false
  paper_has_primary_metric: true
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
---

