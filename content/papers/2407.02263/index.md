---
title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform for Machine Learning
  Force Fields'
arxiv_id: '2407.02263'
source_url: ''
authors:
- name: Shihao Shao
  orcid: null
  s2_author_id: '2140533011'
  s2_url: null
- name: Haoran Geng
  orcid: null
  s2_author_id: '2144742582'
  s2_url: null
- name: Zun Wang
  orcid: null
  s2_author_id: '2189440018'
  s2_url: null
- name: Qinghua Cui
  orcid: null
  s2_author_id: '2143389789'
  s2_url: null
published_date: Jul 2, 2024
published_date_iso: '2024-07-02'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Machine Learning Force Fields (MLFFs) are of great importance for chemistry,
  physics, materials science, and many other related fields. The Clebsch–Gordan Transform
  (CG transform) effectively encodes many-body interactions and is thus an important
  building block for many models of MLFFs. However, the permutation-equivariance requirement
  of MLFFs limits the design space of CG transform, that is, intensive CG transform
  has to be conducted for each neighboring edge and the operations should be performed
  in the same manner for all edges. This constraint results in reduced expressiveness
  of the model while simultaneously increasing computational demands. To overcome
  this challenge, we first implement the CG transform layer on the permutation-invariant
  abstract edges generated from real edge information. We show that this approach
  allows complete freedom in the design of the layer without compromising the crucial
  symmetry. Developing on this free design space, we further propose group CG transform
  with sparse path, abstract edges shuffling, and attention enhancer to form a powerful
  and efficient CG transform layer. Our method, known as FreeCG, achieves state-of-the-art
  (SOTA) results in force prediction for MD17, rMD17, MD22, and is well extended to
  property prediction in QM9 datasets with several improvements greater than 15$\
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- FreeCG
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
  - model: FreeCG
    model_key: freecg
    model_plain: FreeCG
    value: 0.034
    std: null
    paper_value: 0.034
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
    sort_value: 0.034
    sort_std: null
    global_rank: 15
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
  - model: ViSNet
    model_key: visnet
    model_plain: ViSNet
    value: 0.0007
    std: null
    paper_value: 0.0007
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.039
    at_pub_std: null
    at_pub_source_arxiv: '2210.16518'
    at_pub_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural network
      with vector-scalar interactive message passing for molecules'
    at_pub_source_date_iso: '2022-10-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0383
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.039
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 0.0383
    has_value_note: false
    value_note: ''
    sort_value: 0.039
    sort_std: null
    global_rank: 19
    paper_rank: 5
    rank_delta: -14
    rank_delta_abs: 14
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    comparison_source_arxiv: '2210.16518'
    is_best: false
    is_std_outlier: false
  - model: GemNet
    model_key: gemnet
    model_plain: GemNet
    value: 0.131
    std: null
    paper_value: 0.131
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.0502
    at_pub_std: null
    at_pub_source_arxiv: '2402.04836'
    at_pub_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    at_pub_source_date_iso: '2024-02-07'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.08080000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0502
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: false
    value_gap: 0.08080000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.0502
    sort_std: null
    global_rank: 28
    paper_rank: 64
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    comparison_source_arxiv: '2402.04836'
    is_best: false
    is_std_outlier: false
  - model: ET
    model_key: et
    model_plain: ET
    value: 0.123
    std: null
    paper_value: 0.123
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.052
    at_pub_std: null
    at_pub_source_arxiv: '2202.02541'
    at_pub_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    at_pub_source_date_iso: '2022-01-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07100000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.052
    true_std: null
    value_gap_source_arxiv: '2202.02541'
    value_gap_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    value_gap_source_is_current_paper: false
    value_gap: 0.07100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: null
    global_rank: 30
    paper_rank: 63
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    comparison_source_arxiv: '2202.02541'
    is_best: false
    is_std_outlier: false
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
    value: 0.0009
    std: null
    paper_value: 0.0009
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.04
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.0391
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.053
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: false
    value_gap: 0.0521
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 34
    paper_rank: 5
    rank_delta: -29
    rank_delta_abs: 29
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    comparison_source_arxiv: '2205.14276'
    is_best: false
    is_std_outlier: false
  - model: Allegro
    model_key: allegro
    model_plain: Allegro
    value: 0.0046
    std: null
    paper_value: 0.0046
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
    source_ref: musaelian2023learning
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.029
    at_pub_std: null
    at_pub_source_arxiv: '2306.09375'
    at_pub_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    at_pub_source_date_iso: '2023-06-15'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0244
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
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
    value_gap: 0.0484
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 35
    paper_rank: 10
    rank_delta: -25
    rank_delta_abs: 25
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
    is_best: false
    is_std_outlier: false
  - model: BOTNet
    model_key: botnet
    model_plain: BOTNet
    value: 0.0007
    std: null
    paper_value: 0.0007
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
    source_ref: batatia2022design
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.03
    at_pub_std: null
    at_pub_source_arxiv: '2205.06643'
    at_pub_source_title: The design space of E(3)-equivariant atom-centred interatomic
      potentials
    at_pub_source_date_iso: '2022-05-13'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0293
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
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
    value_gap: 0.0523
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 36
    paper_rank: 5
    rank_delta: -31
    rank_delta_abs: 31
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: The design space of E(3)-equivariant atom-centred interatomic
      potentials
    comparison_source_arxiv: '2205.06643'
    is_best: false
    is_std_outlier: false
  - model: UNiTE
    model_key: unite
    model_plain: UNiTE
    value: 0.002
    std: null
    paper_value: 0.002
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
    source_ref: qiao2022informing
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.055
    at_pub_std: null
    at_pub_source_arxiv: '2210.16518'
    at_pub_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural network
      with vector-scalar interactive message passing for molecules'
    at_pub_source_date_iso: '2022-10-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.053
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.055
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 0.053
    has_value_note: false
    value_note: ''
    sort_value: 0.055
    sort_std: null
    global_rank: 38
    paper_rank: 6
    rank_delta: -32
    rank_delta_abs: 32
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    comparison_source_arxiv: '2210.16518'
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.204
    std: null
    paper_value: 0.204
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.064
    at_pub_std: null
    at_pub_source_arxiv: '2003.03123'
    at_pub_source_title: Directional Message Passing for Molecular Graphs
    at_pub_source_date_iso: '2020-03-06'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.13999999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.064
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: false
    value_gap: 0.13999999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.064
    sort_std: null
    global_rank: 42
    paper_rank: 70
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directional Message Passing for Molecular Graphs
    comparison_source_arxiv: '2003.03123'
    is_best: false
    is_std_outlier: false
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    value: 0.167
    std: null
    paper_value: 0.167
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.01
    at_pub_std: null
    at_pub_source_arxiv: '2306.09375'
    at_pub_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    at_pub_source_date_iso: '2023-06-15'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-11-03'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.157
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.077
    true_std: null
    value_gap_source_arxiv: '2311.02124'
    value_gap_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    value_gap_source_is_current_paper: false
    value_gap: 0.09000000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.077
    sort_std: null
    global_rank: 45
    paper_rank: 69
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
    is_best: false
    is_std_outlier: false
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 0.37
    std: null
    paper_value: 0.37
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.05
    at_pub_std: null
    at_pub_source_arxiv: '1902.08408'
    at_pub_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    at_pub_source_date_iso: '2019-02-22'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.32
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.08
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: false
    value_gap: 0.29
    has_value_note: false
    value_note: ''
    sort_value: 0.08
    sort_std: null
    global_rank: 46
    paper_rank: 79
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    comparison_source_arxiv: '1902.08408'
    is_best: false
    is_std_outlier: false
  - model: QuinNet
    model_key: quinnet
    model_plain: QuinNet
    value: 0.119
    std: null
    paper_value: 0.119
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
    sort_value: 0.119
    sort_std: null
    global_rank: 61
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
  - model: So3krates
    model_key: so3krates
    model_plain: So3krates
    value: 0.139
    std: null
    paper_value: 0.139
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.052
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08700000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.139
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.139
    sort_std: null
    global_rank: 65
    paper_rank: 65
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    comparison_source_arxiv: '2205.14276'
    is_best: false
    is_std_outlier: false
  - model: SpookeyNet
    model_key: spookeynet
    model_plain: SpookeyNet
    value: 0.151
    std: null
    paper_value: 0.151
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
    sort_value: 0.151
    sort_std: null
    global_rank: 69
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
single_proposed_model: FreeCG
main_figure: /figures/2407.02263/main_figure.jpegoptim.jpg
---

