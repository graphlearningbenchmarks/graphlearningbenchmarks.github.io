---
title: Efficient and Scalable Density Functional Theory Hamiltonian Prediction through
  Adaptive Sparsity
arxiv_id: '2502.01171'
source_url: ''
authors:
- name: Erpai Luo
  orcid: null
  s2_author_id: '2186682345'
  s2_url: null
- name: Xinran Wei
  orcid: null
  s2_author_id: '2110849142'
  s2_url: null
- name: Lin Huang
  orcid: null
  s2_author_id: '2326207974'
  s2_url: null
- name: Yunyang Li
  orcid: null
  s2_author_id: '2343705389'
  s2_url: null
- name: Hang Yang
  orcid: null
  s2_author_id: '2166223335'
  s2_url: null
- name: Zun Wang
  orcid: null
  s2_author_id: '2108306910'
  s2_url: null
- name: Chang Liu
  orcid: null
  s2_author_id: '2343508559'
  s2_url: null
- name: Zaishuo Xia
  orcid: null
  s2_author_id: '2314368213'
  s2_url: null
- name: Jia Zhang
  orcid: null
  s2_author_id: '2295677107'
  s2_url: null
- name: Bin Shao
  orcid: null
  s2_author_id: '2307007504'
  s2_url: null
published_date: Feb 3, 2025
published_date_iso: '2025-02-03'
published_venue: ICML 2025
published_conference: ICML 2025
published_conference_short: ICML
published_conference_slug: icml
abstract: Hamiltonian matrix prediction is pivotal in computational chemistry, serving
  as the foundation for determining a wide range of molecular properties. While SE(3)
  equivariant graph neural networks have achieved remarkable success in this domain,
  their substantial computational cost--driven by high-order tensor product (TP) operations--restricts
  their scalability to large molecular systems with extensive basis sets. To address
  this challenge, we introduce SPHNet, an efficient and scalable equivariant network,
  that incorporates adaptive SParsity into Hamiltonian prediction. SPHNet employs
  two innovative sparse gates to selectively constrain non-critical interaction combinations,
  significantly reducing tensor product computations while maintaining accuracy. To
  optimize the sparse representation, we develop a Three-phase Sparsity Scheduler,
  ensuring stable convergence and achieving high performance at sparsity rates of
  up to 70%. Extensive evaluations on QH9 and PubchemQH datasets demonstrate that
  SPHNet achieves state-of-the-art accuracy while providing up to a 7x speedup over
  existing models. Beyond Hamiltonian prediction, the proposed sparsification techniques
  also hold significant potential for improving the efficiency and scalability of
  other SE(3) equivariant networks, further broadening their applicability and impact.
  Our code can be found at https://github.com/microsoft/SPHNet.
codebase_url: https://github.com/microsoft/SPHNet
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SPHNet
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
  dataset: MD17
  is_multi_metric: true
  rows:
  - model: PhiSNet (ori)
    model_key: phisnet (ori)
    model_plain: PhiSNet (ori)
    metric_values:
    - 1.073e-05
    - null
    - null
    - null
    metric_stds:
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
    arxiv_id: '2406.03794'
    title: Infusing Self-Consistency into Density Functional Theory Hamiltonian Prediction
      via Deep Equilibrium Models
    published_venue: ''
    date: Jun 6, 2024
    date_display: Jun 2024
    date_iso: '2024-06-06'
    codebase_url: https://github.com/Zun-Wang/DEQHNet
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 1.073e-05
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
  - model: QHNet
    model_key: qhnet
    model_plain: QHNet
    metric_values:
    - null
    - 1.079e-05
    - 3.376e-05
    - 0.9999
    metric_stds:
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
    sort_value: 1.079e-05
    sort_std: null
    true_value: 1.079e-05
    true_std: null
    paper_value: 1.079e-05
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2502.01171'
    value_gap_source_title: Efficient and Scalable Density Functional Theory Hamiltonian
      Prediction through Adaptive Sparsity
    value_note: ''
    at_pub_value: 1.079e-05
    at_pub_std: null
    at_pub_source_arxiv: '2406.03794'
    at_pub_source_title: Infusing Self-Consistency into Density Functional Theory
      Hamiltonian Prediction via Deep Equilibrium Models
    at_pub_source_date_iso: '2024-06-06'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-02-03'
    value_gap_source_date_label: ICML 2025
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
    published_venue: ICML 2025
    date: Feb 3, 2025
    date_display: Feb 2025
    date_iso: '2025-02-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: DEQHNet
    model_key: deqhnet
    model_plain: DEQHNet
    metric_values:
    - 1.507e-05
    - null
    - null
    - null
    metric_stds:
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
    arxiv_id: '2406.03794'
    title: Infusing Self-Consistency into Density Functional Theory Hamiltonian Prediction
      via Deep Equilibrium Models
    published_venue: ''
    date: Jun 6, 2024
    date_display: Jun 2024
    date_iso: '2024-06-06'
    codebase_url: https://github.com/Zun-Wang/DEQHNet
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 1.507e-05
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
  - model: PhiSNet
    model_key: phisnet
    model_plain: PhiSNet
    metric_values:
    - null
    - 1.567e-05
    - 8.553e-05
    - 1.0
    metric_stds:
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
    sort_value: 1.567e-05
    sort_std: null
    true_value: 1.567e-05
    true_std: null
    paper_value: 1.567e-05
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2502.01171'
    value_gap_source_title: Efficient and Scalable Density Functional Theory Hamiltonian
      Prediction through Adaptive Sparsity
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-03'
    value_gap_source_date_label: ICML 2025
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
    published_venue: ICML 2025
    date: Feb 3, 2025
    date_display: Feb 2025
    date_iso: '2025-02-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: SPHNet
    model_key: sphnet
    model_plain: SPHNet
    metric_values:
    - null
    - 1.936e-05
    - 8.23e-05
    - 1.0
    metric_stds:
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
    sort_value: 1.936e-05
    sort_std: null
    true_value: 1.936e-05
    true_std: null
    paper_value: 1.936e-05
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2502.01171'
    value_gap_source_title: Efficient and Scalable Density Functional Theory Hamiltonian
      Prediction through Adaptive Sparsity
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-03'
    value_gap_source_date_label: ICML 2025
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
    published_venue: ICML 2025
    date: Feb 3, 2025
    date_display: Feb 2025
    date_iso: '2025-02-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: SchNOrb
    model_key: schnorb
    model_plain: SchNOrb
    metric_values:
    - null
    - 0.0001654
    - 0.0002793
    - 1.0
    metric_stds:
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
    sort_value: 0.0001654
    sort_std: null
    true_value: 0.0001654
    true_std: null
    paper_value: 0.0001654
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2502.01171'
    value_gap_source_title: Efficient and Scalable Density Functional Theory Hamiltonian
      Prediction through Adaptive Sparsity
    value_note: ''
    at_pub_value: 0.0001654
    at_pub_std: null
    at_pub_source_arxiv: '2406.03794'
    at_pub_source_title: Infusing Self-Consistency into Density Functional Theory
      Hamiltonian Prediction via Deep Equilibrium Models
    at_pub_source_date_iso: '2024-06-06'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-02-03'
    value_gap_source_date_label: ICML 2025
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
    published_venue: ICML 2025
    date: Feb 3, 2025
    date_display: Feb 2025
    date_iso: '2025-02-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  metrics:
  - MAE
  - H
  - epsilon
  - psi
  primary_metric: MAE
  rank_metric: H
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - H
  - epsilon
  - psi
  metric: H
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
    - dataset: MD17
      dataset_slug: md17
single_proposed_model: SPHNet
main_figure: /figures/2502.01171/main_figure.jpegoptim.jpg
---

