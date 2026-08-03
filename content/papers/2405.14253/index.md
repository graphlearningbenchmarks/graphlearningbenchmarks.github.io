---
title: Higher-Rank Irreducible Cartesian Tensors for Equivariant Message Passing
arxiv_id: '2405.14253'
source_url: ''
authors:
- name: V. Zaverkin
  orcid: null
  s2_author_id: '115919348'
  s2_url: null
- name: Francesco Alesiani
  orcid: null
  s2_author_id: '2244943838'
  s2_url: null
- name: Takashi Maruyama
  orcid: null
  s2_author_id: '2276610936'
  s2_url: null
- name: Federico Errica
  orcid: null
  s2_author_id: '41216883'
  s2_url: null
- name: Henrik Christiansen
  orcid: null
  s2_author_id: '2269473709'
  s2_url: null
- name: Makoto Takamoto
  orcid: null
  s2_author_id: '2269471687'
  s2_url: null
- name: Nicolas Weber
  orcid: null
  s2_author_id: '2060123416'
  s2_url: null
- name: Mathias Niepert
  orcid: null
  s2_author_id: '2261287755'
  s2_url: null
published_date: May 23, 2024
published_date_iso: '2024-05-23'
published_venue: NeurIPS 2024
published_conference: NeurIPS 2024
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: The ability to perform fast and accurate atomistic simulations is crucial
  for advancing the chemical sciences. By learning from high-quality data, machine-learned
  interatomic potentials achieve accuracy on par with ab initio and first-principles
  methods at a fraction of their computational cost. The success of machine-learned
  interatomic potentials arises from integrating inductive biases such as equivariance
  to group actions on an atomic system, e.g., equivariance to rotations and reflections.
  In particular, the field has notably advanced with the emergence of equivariant
  message passing. Most of these models represent an atomic system using spherical
  tensors, tensor products of which require complicated numerical coefficients and
  can be computationally demanding. Cartesian tensors offer a promising alternative,
  though state-of-the-art methods lack flexibility in message-passing mechanisms,
  restricting their architectures and expressive power. This work explores higher-rank
  irreducible Cartesian tensors to address these limitations. We integrate irreducible
  Cartesian tensor products into message-passing neural networks and prove the equivariance
  and traceless property of the resulting layers. Through empirical evaluations on
  various benchmark data sets, we consistently observe on-par or better performance
  than that of state-of-the-art spherical and Cartesian models.
codebase_url: https://github.com/nec-research/ictp
extraction_model: google/gemma-4-31B-it
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
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
  rows:
  - model: SliDe
    model_key: qhnet
    model_plain: SliDe
    value: 1.036e-05
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    venue: arXiv.org
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 1.036e-05
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SliDe
    model_key: qhnetv2
    model_plain: SliDe
    value: 1.038e-05
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    venue: arXiv.org
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 1.038e-05
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SliDe
    model_key: phisnet
    model_plain: SliDe
    value: 1.759e-05
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    venue: arXiv.org
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 1.759e-05
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MACE
    model_key: mace
    model_plain: MACE
    value: 2.2
    std: null
    paper_value: 2.2
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    source_ref: Batatia 2022
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 23, 2024
    date_display: May 2024
    date_iso: '2024-05-23'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.0069
    at_pub_std: null
    at_pub_source_arxiv: '2402.04836'
    at_pub_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    at_pub_source_date_iso: '2024-02-07'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 2.1931000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0507
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 2.1493
    has_value_note: false
    value_note: ''
    sort_value: 0.0507
    sort_std: null
    global_rank: 24
    paper_rank: 65
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    comparison_source_arxiv: '2402.04836'
    is_best: false
    is_std_outlier: false
  - model: Allegro
    model_key: allegro
    model_plain: Allegro
    value: 2.3
    std: null
    paper_value: 2.3
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    source_ref: Musaelian 2023
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 23, 2024
    date_display: May 2024
    date_iso: '2024-05-23'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.029
    at_pub_std: null
    at_pub_source_arxiv: '2306.09375'
    at_pub_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    at_pub_source_date_iso: '2023-06-15'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 2.271
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.053
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 2.247
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 29
    paper_rank: 65
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
    is_best: false
    is_std_outlier: false
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
    value: 2.3
    std: null
    paper_value: 2.3
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    source_ref: Batzner 2022
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 23, 2024
    date_display: May 2024
    date_iso: '2024-05-23'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.0009
    at_pub_std: null
    at_pub_source_arxiv: '2402.04836'
    at_pub_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    at_pub_source_date_iso: '2024-02-07'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 2.2990999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.131
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 2.1689999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.131
    sort_std: null
    global_rank: 45
    paper_rank: 65
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    comparison_source_arxiv: '2402.04836'
    is_best: false
    is_std_outlier: false
  - model: ICTP_sym
    model_key: ictp_sym
    model_plain: ICTP_sym
    value: 2.27
    std: 0.11
    paper_value: 2.27
    paper_std: 0.11
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 23, 2024
    date_display: May 2024
    date_iso: '2024-05-23'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 2.27
    sort_std: 0.11
    global_rank: 66
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TensorNet
    model_key: tensornet
    model_plain: TensorNet
    value: 2.4
    std: null
    paper_value: 2.4
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    source_ref: Simeon 2023
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 23, 2024
    date_display: May 2024
    date_iso: '2024-05-23'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 2.4
    sort_std: null
    global_rank: 67
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
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
    - dataset: MD17
      dataset_slug: md17
---

