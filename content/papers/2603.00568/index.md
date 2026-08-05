---
title: Enhancing Molecular Property Predictions by Learning from Bond Modelling and
  Interactions
arxiv_id: '2603.00568'
source_url: ''
authors:
- name: Yunqing Liu
  orcid: null
  s2_author_id: '2280359924'
  s2_url: null
- name: Yi Zhou
  orcid: null
  s2_author_id: '2340939151'
  s2_url: null
- name: Wenqi Fan
  orcid: null
  s2_author_id: '2255025428'
  s2_url: null
published_date: Feb 28, 2026
published_date_iso: '2026-02-28'
published_venue: ICLR 2026
published_conference: ICLR 2026
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Molecule representation learning is crucial for understanding and predicting
  molecular properties. However, conventional atom-centric models, which treat chemical
  bonds merely as pairwise interactions, often overlook complex bond-level phenomena
  like resonance and stereoselectivity. This oversight limits their predictive accuracy
  for nuanced chemical behaviors. To address this limitation, we introduce DeMol,
  a dual-graph framework whose architecture is motivated by a rigorous information-theoretic
  analysis demonstrating the information gain from a bond-centric perspective. DeMol
  explicitly models molecules through parallel atom-centric and bond-centric channels.
  These are synergistically fused by multi-scale Double-Helix Blocks designed to learn
  intricate atom-atom, atom-bond, and bond-bond interactions. The framework's geometric
  consistency is further enhanced by a regularization term based on covalent radii
  to enforce chemically plausible structures. Comprehensive evaluations on diverse
  benchmarks, including PCQM4Mv2, OC20 IS2RE, QM9, and MoleculeNet, show that DeMol
  establishes a new state-of-the-art, outperforming existing methods. These results
  confirm the superiority of explicitly modelling bond information and interactions,
  paving the way for more robust and accurate molecular machine learning.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DeMol
mrr: 1.0
adjusted_mrr: 0.3333
mrr_dataset_count: 1
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: PCQM4Mv2
  rows:
  - model: DeMol
    model_key: demol
    model_plain: DeMol
    value: 0.0603
    std: null
    paper_value: 0.0603
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 186.0
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0603
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0603
    sort_std: null
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TGT-At
    model_key: tgt-at
    model_plain: TGT-At
    value: 0.0671
    std: null
    paper_value: 0.0671
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 203.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0671
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0671
    sort_std: null
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniMol
    model_key: unimol
    model_plain: UniMol
    value: 0.0693
    std: null
    paper_value: 0.0693
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 77.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0693
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0693
    sort_std: null
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Transformer-M
    model_key: transformer-m
    model_plain: Transformer-M
    value: 0.0772
    std: null
    paper_value: 0.0772
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 69.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.0787
    at_pub_std: null
    at_pub_source_arxiv: '2210.01765'
    at_pub_source_title: One Transformer Can Understand Both 2D & 3D Molecular Data
    at_pub_source_date_iso: '2022-10-04'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 0.0015000000000000013
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0772
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0772
    sort_std: null
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: One Transformer Can Understand Both 2D & 3D Molecular
      Data
    comparison_source_arxiv: '2210.01765'
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.0778
    std: null
    paper_value: 0.0778
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 44.3
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 72.0
    at_pub_std: null
    at_pub_source_arxiv: '2402.04538'
    at_pub_source_title: 'Triplet Interaction Improves Graph Transformers: Accurate
      Molecular Graph Learning with Triplet Graph Transformers'
    at_pub_source_date_iso: '2024-02-07'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 71.9222
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0778
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0778
    sort_std: null
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Triplet Interaction Improves Graph Transformers: Accurate
      Molecular Graph Learning with Triplet Graph Transformers'
    comparison_source_arxiv: '2402.04538'
    is_best: false
    is_std_outlier: false
  - model: GEM-2
    model_key: gem-2
    model_plain: GEM-2
    value: 0.0793
    std: null
    paper_value: 0.0793
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 32.1
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.0806
    at_pub_std: null
    at_pub_source_arxiv: '2208.05863'
    at_pub_source_title: 'GEM-2: Next Generation Molecular Property Prediction Network
      by Modeling Full-range Many-body Interactions'
    at_pub_source_date_iso: '2022-08-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 0.0013000000000000095
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0793
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0793
    sort_std: null
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GEM-2: Next Generation Molecular Property Prediction
      Network by Modeling Full-range Many-body Interactions'
    comparison_source_arxiv: '2208.05863'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS_DEEP
    model_key: graphgps_deep
    model_plain: GraphGPS_DEEP
    value: 0.0852
    std: null
    paper_value: 0.0852
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 13.8
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0852
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0852
    sort_std: null
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS_BASE
    model_key: graphgps_base
    model_plain: GraphGPS_BASE
    value: 0.0858
    std: null
    paper_value: 0.0858
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.4
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.0858
    at_pub_std: null
    at_pub_source_arxiv: '2210.01765'
    at_pub_source_title: One Transformer Can Understand Both 2D & 3D Molecular Data
    at_pub_source_date_iso: '2022-10-04'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0858
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0858
    sort_std: null
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
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.0869
    std: null
    paper_value: 0.0869
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 89.3
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.0862
    at_pub_std: null
    at_pub_source_arxiv: '2208.05863'
    at_pub_source_title: 'GEM-2: Next Generation Molecular Property Prediction Network
      by Modeling Full-range Many-body Interactions'
    at_pub_source_date_iso: '2022-08-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-08-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0007000000000000062
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0862
    true_std: null
    value_gap_source_arxiv: '2208.05863'
    value_gap_source_title: 'GEM-2: Next Generation Molecular Property Prediction
      Network by Modeling Full-range Many-body Interactions'
    value_gap_source_is_current_paper: false
    value_gap: 0.0007000000000000062
    has_value_note: false
    value_note: ''
    sort_value: 0.0862
    sort_std: null
    global_rank: 26
    paper_rank: 29
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GEM-2: Next Generation Molecular Property Prediction
      Network by Modeling Full-range Many-body Interactions'
    comparison_source_arxiv: '2208.05863'
    is_best: false
    is_std_outlier: false
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.0864
    std: null
    paper_value: 0.0864
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 47.1
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.0864
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0864
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0864
    sort_std: null
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRPE_LARGE
    model_key: grpe_large
    model_plain: GRPE_LARGE
    value: 0.0867
    std: null
    paper_value: 0.0867
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.0867
    at_pub_std: null
    at_pub_source_arxiv: '2210.01765'
    at_pub_source_title: One Transformer Can Understand Both 2D & 3D Molecular Data
    at_pub_source_date_iso: '2022-10-04'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0867
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0867
    sort_std: null
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRPE_BASE
    model_key: grpe_base
    model_plain: GRPE_BASE
    value: 0.089
    std: null
    paper_value: 0.089
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.089
    at_pub_std: null
    at_pub_source_arxiv: '2210.01765'
    at_pub_source_title: One Transformer Can Understand Both 2D & 3D Molecular Data
    at_pub_source_date_iso: '2022-10-04'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.089
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.089
    sort_std: null
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TokenGT
    model_key: tokengt
    model_plain: TokenGT
    value: 0.091
    std: null
    paper_value: 0.091
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 48.5
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.091
    at_pub_std: null
    at_pub_source_arxiv: '2210.01765'
    at_pub_source_title: One Transformer Can Understand Both 2D & 3D Molecular Data
    at_pub_source_date_iso: '2022-10-04'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.091
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.091
    sort_std: null
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
  - model: GraphGPS_SMALL
    model_key: graphgps_small
    model_plain: GraphGPS_SMALL
    value: 0.0938
    std: null
    paper_value: 0.0938
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.2
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.0938
    at_pub_std: null
    at_pub_source_arxiv: '2210.01765'
    at_pub_source_title: One Transformer Can Understand Both 2D & 3D Molecular Data
    at_pub_source_date_iso: '2022-10-04'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0938
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0938
    sort_std: null
    global_rank: 49
    paper_rank: 49
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeeperGCN-VN
    model_key: deepergcn-vn
    model_plain: DeeperGCN-VN
    value: 0.1021
    std: null
    paper_value: 0.1021
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 25.5
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.1021
    at_pub_std: null
    at_pub_source_arxiv: '2210.01765'
    at_pub_source_title: One Transformer Can Understand Both 2D & 3D Molecular Data
    at_pub_source_date_iso: '2022-10-04'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1021
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1021
    sort_std: null
    global_rank: 52
    paper_rank: 52
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN-VN
    model_key: gin-vn
    model_plain: GIN-VN
    value: 0.1083
    std: null
    paper_value: 0.1083
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.7
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.1083
    at_pub_std: null
    at_pub_source_arxiv: '2207.02505'
    at_pub_source_title: Pure Transformers are Powerful Graph Learners
    at_pub_source_date_iso: '2022-07-06'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1083
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1083
    sort_std: null
    global_rank: 55
    paper_rank: 55
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN-VN
    model_key: gcn-vn
    model_plain: GCN-VN
    value: 0.1153
    std: null
    paper_value: 0.1153
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 4.9
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.1152
    at_pub_std: null
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-05-19'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: 0.00010000000000000286
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1152
    true_std: null
    value_gap_source_arxiv: '2305.11424'
    value_gap_source_title: IJCAI--23 Formatting Instructions
    value_gap_source_is_current_paper: false
    value_gap: 0.00010000000000000286
    has_value_note: false
    value_note: ''
    sort_value: 0.1152
    sort_std: null
    global_rank: 57
    paper_rank: 58
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    comparison_source_arxiv: '2201.12787'
    is_best: false
    is_std_outlier: false
  - model: GINE-VN
    model_key: gine-vn
    model_plain: GINE-VN
    value: 0.1167
    std: null
    paper_value: 0.1167
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 13.2
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.1167
    at_pub_std: null
    at_pub_source_arxiv: '2210.01765'
    at_pub_source_title: One Transformer Can Understand Both 2D & 3D Molecular Data
    at_pub_source_date_iso: '2022-10-04'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1167
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1167
    sort_std: null
    global_rank: 59
    paper_rank: 59
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
    value: 0.1379
    std: null
    paper_value: 0.1379
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 2.0
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.1195
    at_pub_std: null
    at_pub_source_arxiv: '2310.20519'
    at_pub_source_title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    at_pub_source_date_iso: '2023-10-31'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-31'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0184
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1195
    true_std: null
    value_gap_source_arxiv: '2310.20519'
    value_gap_source_title: Enhancing Graph Neural Networks with Quantum Computed
      Encodings
    value_gap_source_is_current_paper: false
    value_gap: 0.0184
    has_value_note: false
    value_note: ''
    sort_value: 0.1195
    sort_std: null
    global_rank: 63
    paper_rank: 73
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Enhancing Graph Neural Networks with Quantum Computed
      Encodings
    comparison_source_arxiv: '2310.20519'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.1195
    std: null
    paper_value: 0.1195
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.8
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
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.1195
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1195
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1195
    sort_std: null
    global_rank: 62
    paper_rank: 62
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP-Fingerprint
    model_key: mlp-fingerprint
    model_plain: MLP-Fingerprint
    value: 0.1735
    std: null
    paper_value: 0.1735
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.1
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.1753
    at_pub_std: null
    at_pub_source_arxiv: '2210.01765'
    at_pub_source_title: One Transformer Can Understand Both 2D & 3D Molecular Data
    at_pub_source_date_iso: '2022-10-04'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 0.0018000000000000238
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1735
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1735
    sort_std: null
    global_rank: 80
    paper_rank: 80
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: One Transformer Can Understand Both 2D & 3D Molecular
      Data
    comparison_source_arxiv: '2210.01765'
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
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: PCQM4Mv2
      dataset_slug: pcqm4mv2
single_proposed_model: DeMol
main_figure: /figures/2603.00568/main_figure.jpegoptim.jpg
---

