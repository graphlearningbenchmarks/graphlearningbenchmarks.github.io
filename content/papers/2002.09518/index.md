---
title: Memory-Based Graph Networks
arxiv_id: '2002.09518'
source_url: ''
authors:
- name: Amir Hosein Khas Ahmadi
  orcid: null
  s2_author_id: '1516916058'
  s2_url: null
- name: Kaveh Hassani
  orcid: null
  s2_author_id: '2443055'
  s2_url: null
- name: Parsa Moradi
  orcid: null
  s2_author_id: '3249115'
  s2_url: null
- name: Leo J. Lee
  orcid: null
  s2_author_id: '2258684419'
  s2_url: null
- name: Q. Morris
  orcid: null
  s2_author_id: '2058740157'
  s2_url: null
published_date: Feb 21, 2020
published_date_iso: '2020-02-21'
published_venue: ICLR 2020
published_conference: ICLR 2020
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'Graph neural networks (GNNs) are a class of deep models that operate on
  data with arbitrary topology represented as graphs. We introduce an efficient memory
  layer for GNNs that can jointly learn node representations and coarsen the graph.
  We also introduce two new networks based on this layer: memory-based GNN (MemGNN)
  and graph memory network (GMN) that can learn hierarchical graph representations.
  The experimental results show that the proposed models achieve state-of-the-art
  results in eight out of nine graph classification and regression benchmarks. We
  also show that the learned representations could correspond to chemical features
  in the molecule data. Code and reference implementations are released at: https://github.com/amirkhas/GraphMemoryNet'
codebase_url: https://github.com/amirkhas/GraphMemoryNet
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GMN
- MemGNN
mrr: 0.4472
adjusted_mrr: 0.4472
mrr_dataset_count: 3
benchmark_categories:
- TU Dortmund
- MoleculeNet
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 3
  total: 11
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 4
  total: 9
task_categories:
- graph_classification
- graph_regression
experiment_scopes:
- graph-level
results:
- &id005
  dataset: BACE
  rows:
  - model: ProtoMol
    model_key: protomol
    model_plain: ProtoMol
    value: 0.914
    std: 0.003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.16824'
    title: 'ProtoMol: Enhancing Molecular Property Prediction via Prototype-Guided
      Multimodal Learning'
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    venue: Briefings Bioinform.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.914
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MMSG
    model_key: mmsg
    model_plain: MMSG
    value: 0.908
    std: 0.005
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.16824'
    title: 'ProtoMol: Enhancing Molecular Property Prediction via Prototype-Guided
      Multimodal Learning'
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    venue: Briefings Bioinform.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.908
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.907
    std: 0.0
    paper_value: 0.907
    paper_std: 0.0
    metric: ROC-AUC
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
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.907
    true_std: 0.0
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.907
    sort_std: 0.0
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
  - model: Random Forest
    model_key: random forest
    model_plain: Random Forest
    value: 0.867
    std: 0.008
    paper_value: 0.867
    paper_std: 0.008
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.867
    true_std: 0.008
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.867
    sort_std: 0.008
    global_rank: 38
    paper_rank: 38
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
    value: 0.8646
    std: 0.0081
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.15589'
    title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
      Graph Information Bottleneck
    date: Dec 20, 2024
    date_display: Dec 2024
    date_iso: '2024-12-20'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/NSLab-CUK/S-CGIB
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 43
    sort_value: 0.8646
    sort_std: 0.0081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Kernel SVM
    model_key: kernel svm
    model_plain: Kernel SVM
    value: 0.862
    std: 0.0
    paper_value: 0.862
    paper_std: 0.0
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.862
    true_std: 0.0
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.862
    sort_std: 0.0
    global_rank: 48
    paper_rank: 48
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
    value: 0.783
    std: 0.014
    paper_value: 0.783
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
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.854
    true_std: 0.011
    value_gap_source_arxiv: '2310.07351'
    value_gap_source_title: Atom-Motif Contrastive Transformer for Molecular Property
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.07099999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.854
    sort_std: 0.011
    global_rank: 64
    paper_rank: 213
    rank_delta: 149
    rank_delta_abs: 149
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: XGBoost
    model_key: xgboost
    model_plain: XGBoost
    value: 0.85
    std: 0.008
    paper_value: 0.85
    paper_std: 0.008
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.85
    true_std: 0.008
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.85
    sort_std: 0.008
    global_rank: 75
    paper_rank: 75
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IRV
    model_key: irv
    model_plain: IRV
    value: 0.838
    std: 0.0
    paper_value: 0.838
    paper_std: 0.0
    metric: ROC-AUC
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.838
    true_std: 0.0
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.838
    sort_std: 0.0
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
  - model: Bypass
    model_key: bypass
    model_plain: Bypass
    value: 0.829
    std: 0.006
    paper_value: 0.829
    paper_std: 0.006
    metric: ROC-AUC
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.829
    true_std: 0.006
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: 0.006
    global_rank: 110
    paper_rank: 110
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Multitask
    model_key: multitask
    model_plain: Multitask
    value: 0.824
    std: 0.0006
    paper_value: 0.824
    paper_std: 0.0006
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
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.824
    true_std: 0.0006
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.824
    sort_std: 0.0006
    global_rank: 123
    paper_rank: 123
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Weave
    model_key: weave
    model_plain: Weave
    value: 0.806
    std: 0.002
    paper_value: 0.806
    paper_std: 0.002
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
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.806
    true_std: 0.002
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.806
    sort_std: 0.002
    global_rank: 168
    paper_rank: 168
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Logistic Regression
    model_key: logistic regression
    model_plain: Logistic Regression
    value: 0.781
    std: 0.01
    paper_value: 0.781
    paper_std: 0.01
    metric: ROC-AUC
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation following wu2018moleculenet protocol
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.781
    true_std: 0.01
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.781
    sort_std: 0.01
    global_rank: 217
    paper_rank: 217
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
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
- &id002
  dataset: COLLAB
  rows:
  - model: WL-MLP
    model_key: wl-mlp
    model_plain: WL-MLP
    value: 0.9792
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9792
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.964
    std: 0.007
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.964
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CoCN
    model_key: cocn
    model_plain: CoCN
    value: 0.8722
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.18480'
    title: Scalable Graph Compressed Convolutions
    date: Jul 26, 2024
    date_display: Jul 2024
    date_iso: '2024-07-26'
    venue: arXiv.org
    codebase_url: https://github.com/sunjss/CoCN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: use the one-hot encoding of node degrees as node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.8722
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.826
    std: 0.022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.11714'
    title: Scalable Expressiveness through Preprocessed Graph Perturbations
    date: Jun 17, 2024
    date_display: Jun 2024
    date_iso: '2024-06-17'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/Danial-sb/SE2P
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 23
    sort_value: 0.826
    sort_std: 0.022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.7548
    std: null
    paper_value: 0.7548
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
    source_ref: ying_2018_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.789
    at_pub_std: 0.023
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2024-07-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03420000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8213
    true_std: 0.0043
    value_gap_source_arxiv: '2407.18480'
    value_gap_source_title: Scalable Graph Compressed Convolutions
    value_gap_source_is_current_paper: false
    value_gap: 0.0665
    has_value_note: false
    value_note: ''
    sort_value: 0.8213
    sort_std: 0.0043
    global_rank: 34
    paper_rank: 262
    rank_delta: 228
    rank_delta_abs: 228
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fast Graph Representation Learning with PyTorch Geometric
    comparison_source_arxiv: '1903.02428'
    is_best: false
    is_std_outlier: false
  - model: TopKPool
    model_key: topkpool
    model_plain: TopKPool
    value: 0.7756
    std: null
    paper_value: 0.7756
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
    source_ref: gao_2019_icml
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.646
    at_pub_std: 0.021
    at_pub_source_arxiv: '1905.10990'
    at_pub_source_title: Edge Contraction Pooling for Graph Neural Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2022-05-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.12959999999999994
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.814
    true_std: 0.0094
    value_gap_source_arxiv: '2205.15068'
    value_gap_source_title: Embedding Graphs on Grassmann Manifold
    value_gap_source_is_current_paper: false
    value_gap: 0.03839999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.814
    sort_std: 0.0094
    global_rank: 58
    paper_rank: 202
    rank_delta: 144
    rank_delta_abs: 144
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Edge Contraction Pooling for Graph Neural Networks
    comparison_source_arxiv: '1905.10990'
    is_best: false
    is_std_outlier: false
  - model: WL Optimal
    model_key: wl optimal
    model_plain: WL Optimal
    value: 0.8074
    std: null
    paper_value: 0.8074
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kriege_2016_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8074
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8074
    sort_std: null
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
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.8018
    std: null
    paper_value: 0.8018
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
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8018
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8018
    sort_std: null
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
  - model: SortPool
    model_key: sortpool
    model_plain: SortPool
    value: 0.7376
    std: null
    paper_value: 0.7376
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
    source_ref: morris_2019_aaai
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.777
    at_pub_std: 0.031
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2021-03-01'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.03939999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8007
    true_std: null
    value_gap_source_arxiv: '2103.00959'
    value_gap_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.06309999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8007
    sort_std: null
    global_rank: 129
    paper_rank: 293
    rank_delta: 164
    rank_delta_abs: 164
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fast Graph Representation Learning with PyTorch Geometric
    comparison_source_arxiv: '1903.02428'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.6825
    std: null
    paper_value: 0.6825
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
    source_ref: hamilton_2017_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.797
    at_pub_std: 0.017
    at_pub_source_arxiv: '1909.11855'
    at_pub_source_title: Universal Graph Transformer Self-Attention Networks
    at_pub_source_date_iso: '2019-09-26'
    at_pub_source_date_label: WWW 2019
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.11450000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.797
    true_std: 0.017
    value_gap_source_arxiv: '2310.11025'
    value_gap_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.11450000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.797
    sort_std: 0.017
    global_rank: 142
    paper_rank: 333
    rank_delta: 191
    rank_delta_abs: 191
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Universal Graph Transformer Self-Attention Networks
    comparison_source_arxiv: '1909.11855'
    is_best: false
    is_std_outlier: false
  - model: Set2Set
    model_key: set2set
    model_plain: Set2Set
    value: 0.7175
    std: null
    paper_value: 0.7175
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
    source_ref: vinyals_2015_iclr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.796
    at_pub_std: 0.023
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-03-06'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.07850000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.796
    true_std: 0.023
    value_gap_source_arxiv: '1903.02428'
    value_gap_source_title: Fast Graph Representation Learning with PyTorch Geometric
    value_gap_source_is_current_paper: false
    value_gap: 0.07850000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.796
    sort_std: 0.023
    global_rank: 148
    paper_rank: 311
    rank_delta: 163
    rank_delta_abs: 163
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fast Graph Representation Learning with PyTorch Geometric
    comparison_source_arxiv: '1903.02428'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.792
    std: 0.024
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 157
    sort_value: 0.792
    sort_std: 0.024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.7861
    std: null
    paper_value: 0.7861
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
    source_ref: shervashidze_2011_jmlr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.791
    at_pub_std: 0.001
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2016-06-03'
    value_gap_source_date_label: NeurIPS 2016
    gap_vs_at_pub: 0.0049000000000000155
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.791
    true_std: 0.001
    value_gap_source_arxiv: '1606.01141'
    value_gap_source_title: On Valid Optimal Assignment Kernels and Applications to
      Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.0049000000000000155
    has_value_note: false
    value_note: ''
    sort_value: 0.791
    sort_std: 0.001
    global_rank: 160
    paper_rank: 174
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Valid Optimal Assignment Kernels and Applications
      to Graph Classification
    comparison_source_arxiv: '1606.01141'
    is_best: false
    is_std_outlier: false
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.77
    std: null
    paper_value: 0.77
    paper_std: null
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
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.77
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.77
    sort_std: null
    global_rank: 224
    paper_rank: 224
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Sparse HGC
    model_key: sparse hgc
    model_plain: Sparse HGC
    value: 0.7546
    std: null
    paper_value: 0.7546
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
    source_ref: cangea_2018_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7546
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7546
    sort_std: null
    global_rank: 263
    paper_rank: 263
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CliquePool
    model_key: cliquepool
    model_plain: CliquePool
    value: 0.745
    std: null
    paper_value: 0.745
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
    source_ref: Luzhnica_2019_iclr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.745
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: null
    global_rank: 280
    paper_rank: 280
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.726
    std: null
    paper_value: 0.726
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
    source_ref: niepert_2016_icml
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.726
    at_pub_std: 0.022
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.726
    true_std: 0.042
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.726
    sort_std: 0.042
    global_rank: 304
    paper_rank: 304
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ECC
    model_key: ecc
    model_plain: ECC
    value: 0.6779
    std: null
    paper_value: 0.6779
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
    source_ref: simonovsky_2017_cvpr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6779
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6779
    sort_std: null
    global_rank: 337
    paper_rank: 337
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.6466
    std: null
    paper_value: 0.6466
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
    source_ref: shervashidze_2009_ais
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6466
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6466
    sort_std: null
    global_rank: 347
    paper_rank: 347
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ShortestPath
    model_key: shortestpath
    model_plain: ShortestPath
    value: 0.591
    std: null
    paper_value: 0.591
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: borgwardt_2005_icdm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.591
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.591
    sort_std: null
    global_rank: 356
    paper_rank: 356
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
  dataset: ENZYMES
  rows:
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.7866
    std: null
    paper_value: 0.7866
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
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7866
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7866
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
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.755
    std: null
    paper_value: 0.755
    paper_std: null
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
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.755
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.755
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
  - model: TFGW SP
    model_key: tfgw sp (l=2)
    model_plain: TFGW SP
    value: 0.751
    std: 0.05
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.751
    sort_std: 0.05
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.7
    std: 0.04944
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 17
    sort_value: 0.7
    sort_std: 0.04944
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.5343
    std: null
    paper_value: 0.5343
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
    source_ref: shervashidze_2011_jmlr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.5905
    at_pub_std: null
    at_pub_source_arxiv: '1704.02901'
    at_pub_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    at_pub_source_date_iso: '2017-04-10'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.05620000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.695
    true_std: 0.032
    value_gap_source_arxiv: '2205.15733'
    value_gap_source_title: Template based Graph Neural Network with Optimal Transport
      Distances
    value_gap_source_is_current_paper: false
    value_gap: 0.16069999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.695
    sort_std: 0.032
    global_rank: 19
    paper_rank: 153
    rank_delta: 134
    rank_delta_abs: 134
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    comparison_source_arxiv: '1704.02901'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.5425
    std: null
    paper_value: 0.5425
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
    source_ref: hamilton_2017_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.603
    at_pub_std: 0.071
    at_pub_source_arxiv: '1901.01343'
    at_pub_source_title: Graph Neural Networks With Convolutional ARMA Filters
    at_pub_source_date_iso: '2019-01-05'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2023-01-01'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: 0.0605
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.68167
    true_std: 0.05449
    value_gap_source_arxiv: '2003.00982'
    value_gap_source_title: GNNBenchmark
    value_gap_source_is_current_paper: false
    value_gap: 0.13917000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.68167
    sort_std: 0.05449
    global_rank: 27
    paper_rank: 147
    rank_delta: 120
    rank_delta_abs: 120
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.67667
    std: 0.05831
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 33
    sort_value: 0.67667
    sort_std: 0.05831
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Sparse HGC
    model_key: sparse hgc
    model_plain: Sparse HGC
    value: 0.6417
    std: null
    paper_value: 0.6417
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
    source_ref: cangea_2018_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6417
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6417
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
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.6053
    std: null
    paper_value: 0.6053
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
    source_ref: ying_2018_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.246
    at_pub_std: 0.053
    at_pub_source_arxiv: '1910.11436'
    at_pub_source_title: Hierarchical Representation Learning in Graph Neural Networks
      with Node Decimation Pooling
    at_pub_source_date_iso: '2019-10-24'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.35929999999999995
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6253
    true_std: null
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: 0.020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.6253
    sort_std: null
    global_rank: 76
    paper_rank: 98
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Hierarchical Representation Learning in Graph Neural
      Networks with Node Decimation Pooling
    comparison_source_arxiv: '1910.11436'
    is_best: false
    is_std_outlier: false
  - model: CliquePool
    model_key: cliquepool
    model_plain: CliquePool
    value: 0.6071
    std: null
    paper_value: 0.6071
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
    source_ref: Luzhnica_2019_iclr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-16'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6071
    true_std: null
    value_gap_source_arxiv: '2012.08734'
    value_gap_source_title: Hierarchical Graph Capsule Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6071
    sort_std: null
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Set2Set
    model_key: set2set
    model_plain: Set2Set
    value: 0.6015
    std: null
    paper_value: 0.6015
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
    source_ref: vinyals_2015_iclr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.38
    at_pub_std: null
    at_pub_source_arxiv: '1904.13107'
    at_pub_source_title: Graph Convolutional Networks with EigenPooling
    at_pub_source_date_iso: '2019-04-30'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.22150000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6015
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6015
    sort_std: null
    global_rank: 101
    paper_rank: 101
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Convolutional Networks with EigenPooling
    comparison_source_arxiv: '1904.13107'
    is_best: false
    is_std_outlier: false
  - model: WL Optimal
    model_key: wl optimal
    model_plain: WL Optimal
    value: 0.6013
    std: null
    paper_value: 0.6013
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kriege_2016_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6013
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6013
    sort_std: null
    global_rank: 102
    paper_rank: 102
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SortPool
    model_key: sortpool
    model_plain: SortPool
    value: 0.5712
    std: null
    paper_value: 0.5712
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
    source_ref: morris_2019_aaai
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5712
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5712
    sort_std: null
    global_rank: 129
    paper_rank: 129
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
    value: 0.55833
    std: 0.03516
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 133
    sort_value: 0.55833
    sort_std: 0.03516
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.4103
    std: null
    paper_value: 0.4103
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
    source_ref: shervashidze_2009_ais
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.1095
    at_pub_std: 0.0069
    at_pub_source_arxiv: '1603.06186'
    at_pub_source_title: The Multiscale Laplacian Graph Kernel
    at_pub_source_date_iso: '2016-03-01'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.3008
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.553
    true_std: 0.0378
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.14270000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.553
    sort_std: 0.0378
    global_rank: 137
    paper_rank: 211
    rank_delta: 74
    rank_delta_abs: 74
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: The Multiscale Laplacian Graph Kernel
    comparison_source_arxiv: '1603.06186'
    is_best: false
    is_std_outlier: false
  - model: ECC
    model_key: ecc
    model_plain: ECC
    value: 0.535
    std: null
    paper_value: 0.535
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
    source_ref: simonovsky_2017_cvpr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.535
    at_pub_std: null
    at_pub_source_arxiv: '1704.02901'
    at_pub_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    at_pub_source_date_iso: '2017-04-10'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.535
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.535
    sort_std: null
    global_rank: 153
    paper_rank: 153
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ShortestPath
    model_key: shortestpath
    model_plain: ShortestPath
    value: 0.4232
    std: null
    paper_value: 0.4232
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: borgwardt_2005_icdm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, mean accuracy reported.
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4232
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4232
    sort_std: null
    global_rank: 206
    paper_rank: 206
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
- &id006
  dataset: ESOL
  rows:
  - model: Graphormer-SPIS
    model_key: graphormer-spis
    model_plain: Graphormer-SPIS
    value: 0.484
    std: 0.005
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_display: May 2023
    date_iso: '2023-05-23'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.484
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPD
    model_key: graphormer-spd
    model_plain: Graphormer-SPD
    value: 0.492
    std: 0.004
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_display: May 2023
    date_iso: '2023-05-23'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.492
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: conan-FGW
    model_key: conan-fgw
    model_plain: conan-FGW
    value: 0.514
    std: 0.019
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_display: Feb 2024
    date_iso: '2024-02-03'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.514
    sort_std: 0.019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.54
    std: 0.01
    paper_value: 0.54
    paper_std: 0.01
    metric: RMSE
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: test split results for ESOL regression
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.54
    true_std: 0.01
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.54
    sort_std: 0.01
    global_rank: 4
    paper_rank: 4
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
    value: 0.97
    std: 0.01
    paper_value: 0.97
    paper_std: 0.01
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: test split results for ESOL regression
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-23'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.564
    true_std: 0.015
    value_gap_source_arxiv: '2305.13987'
    value_gap_source_title: On Structural Expressive Power of Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.406
    has_value_note: false
    value_note: ''
    sort_value: 0.564
    sort_std: 0.015
    global_rank: 7
    paper_rank: 79
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.58
    std: 0.03
    paper_value: 0.58
    paper_std: 0.03
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: test split results for ESOL regression
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.58
    at_pub_std: 0.03
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.58
    true_std: 0.03
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.58
    sort_std: 0.03
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.601
    std: 0.008
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_display: May 2023
    date_iso: '2023-05-23'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 18
    sort_value: 0.601
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Weave
    model_key: weave
    model_plain: Weave
    value: 0.61
    std: 0.07
    paper_value: 0.61
    paper_std: 0.07
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: test split results for ESOL regression
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.61
    at_pub_std: 0.07
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.61
    true_std: 0.07
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.61
    sort_std: 0.07
    global_rank: 20
    paper_rank: 20
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAG
    model_key: dag
    model_plain: DAG
    value: 0.82
    std: 0.08
    paper_value: 0.82
    paper_std: 0.08
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: test split results for ESOL regression
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.82
    at_pub_std: 0.08
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.82
    true_std: 0.08
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.82
    sort_std: 0.08
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
  - model: XGBoost
    model_key: xgboost
    model_plain: XGBoost
    value: 0.99
    std: 0.14
    paper_value: 0.99
    paper_std: 0.14
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: test split results for ESOL regression
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.99
    at_pub_std: 0.14
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2026-04-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.832
    true_std: null
    value_gap_source_arxiv: '2604.06336'
    value_gap_source_title: 'BiScale-GTR: Fragment-Aware Graph Transformers for Multi-Scale
      Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.15800000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.832
    sort_std: null
    global_rank: 54
    paper_rank: 84
    rank_delta: 30
    rank_delta_abs: 30
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Random Forest
    model_key: random forest
    model_plain: Random Forest
    value: 1.07
    std: 0.19
    paper_value: 1.07
    paper_std: 0.19
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: test split results for ESOL regression
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.07
    true_std: 0.19
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.07
    sort_std: 0.19
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
  - model: Multitask
    model_key: multitask
    model_plain: Multitask
    value: 1.12
    std: 0.19
    paper_value: 1.12
    paper_std: 0.19
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: test split results for ESOL regression
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 1.12
    at_pub_std: 0.15
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.12
    true_std: 0.19
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.12
    sort_std: 0.19
    global_rank: 107
    paper_rank: 107
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KRR
    model_key: krr
    model_plain: KRR
    value: 1.53
    std: 0.06
    paper_value: 1.53
    paper_std: 0.06
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: test split results for ESOL regression
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 1.53
    at_pub_std: 0.06
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.53
    true_std: 0.06
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.53
    sort_std: 0.06
    global_rank: 134
    paper_rank: 134
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id007
  dataset: Lipophilicity
  rows:
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.556
    std: 0.023
    paper_value: 0.556
    paper_std: 0.023
    metric: RMSE
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split RMSE for Lipophilicity
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.556
    true_std: 0.023
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.556
    sort_std: 0.023
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
  - model: ProtoS-L2
    model_key: protos-l2
    model_plain: ProtoS-L2
    value: 0.58
    std: 0.016
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.065
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_display: Jun 2020
    date_iso: '2020-06-08'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.58
    sort_std: 0.016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ProtoW-L2
    model_key: protow-l2
    model_plain: ProtoW-L2
    value: 0.604
    std: 0.014
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_display: Jun 2020
    date_iso: '2020-06-08'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.604
    sort_std: 0.014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.655
    std: 0.036
    paper_value: 0.655
    paper_std: 0.036
    metric: RMSE
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split RMSE for Lipophilicity
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.655
    true_std: 0.036
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.655
    sort_std: 0.036
    global_rank: 7
    paper_rank: 7
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
    value: 0.658
    std: 0.019
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.626
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_display: Jun 2020
    date_iso: '2020-06-08'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 9
    sort_value: 0.658
    sort_std: 0.019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.715
    std: 0.035
    paper_value: 0.715
    paper_std: 0.035
    metric: RMSE
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split RMSE for Lipophilicity
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.719
    at_pub_std: 0.031
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2023-07-14'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.712
    true_std: null
    value_gap_source_arxiv: '2307.07107'
    value_gap_source_title: Graph Positional and Structural Encoder
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.712
    sort_std: null
    global_rank: 22
    paper_rank: 24
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Weave
    model_key: weave
    model_plain: Weave
    value: 0.715
    std: 0.035
    paper_value: 0.715
    paper_std: 0.035
    metric: RMSE
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split RMSE for Lipophilicity
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.715
    at_pub_std: 0.035
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.715
    true_std: 0.035
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.715
    sort_std: 0.035
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
  - model: XGBoost
    model_key: xgboost
    model_plain: XGBoost
    value: 0.799
    std: 0.054
    paper_value: 0.799
    paper_std: 0.054
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split RMSE for Lipophilicity
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.799
    at_pub_std: 0.054
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.799
    true_std: 0.054
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.799
    sort_std: 0.054
    global_rank: 57
    paper_rank: 57
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAG
    model_key: dag
    model_plain: DAG
    value: 0.835
    std: 0.039
    paper_value: 0.835
    paper_std: 0.039
    metric: RMSE
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split RMSE for Lipophilicity
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.835
    at_pub_std: 0.039
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.835
    true_std: 0.039
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.835
    sort_std: 0.039
    global_rank: 65
    paper_rank: 65
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Multitask
    model_key: multitask
    model_plain: Multitask
    value: 0.859
    std: 0.013
    paper_value: 0.859
    paper_std: 0.013
    metric: RMSE
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split RMSE for Lipophilicity
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.859
    at_pub_std: 0.013
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.859
    true_std: 0.013
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.859
    sort_std: 0.013
    global_rank: 72
    paper_rank: 72
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Random Forest
    model_key: random forest
    model_plain: Random Forest
    value: 0.876
    std: 0.04
    paper_value: 0.876
    paper_std: 0.04
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split RMSE for Lipophilicity
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.876
    true_std: 0.04
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.876
    sort_std: 0.04
    global_rank: 74
    paper_rank: 74
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KRR
    model_key: krr
    model_plain: KRR
    value: 0.899
    std: 0.043
    paper_value: 0.899
    paper_std: 0.043
    metric: RMSE
    higher_is_better: false
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split RMSE for Lipophilicity
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.899
    at_pub_std: 0.043
    at_pub_source_arxiv: '1703.00564'
    at_pub_source_title: MoleculeNet
    at_pub_source_date_iso: '2017-03-02'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.899
    true_std: 0.043
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.899
    sort_std: 0.043
    global_rank: 80
    paper_rank: 80
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: PROTEINS
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.941
    std: 0.033
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.941
    sort_std: 0.033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GRDL
    model_key: grdl
    model_plain: GRDL
    value: 0.826
    std: 0.012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.11370'
    title: 'Graph Classification via Reference Distribution Learning: Theory and Practice'
    date: Aug 21, 2024
    date_display: Aug 2024
    date_iso: '2024-08-21'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.826
    sort_std: 0.012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.8225
    std: null
    paper_value: 0.8225
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
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8225
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8225
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
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.7625
    std: null
    paper_value: 0.7625
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
    source_ref: ying_2018_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.751
    at_pub_std: 0.035
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.011499999999999955
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8161
    true_std: 0.0232
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.05360000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.8161
    sort_std: 0.0232
    global_rank: 7
    paper_rank: 154
    rank_delta: 147
    rank_delta_abs: 147
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.8135
    std: null
    paper_value: 0.8135
    paper_std: null
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
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8135
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8135
    sort_std: null
    global_rank: 9
    paper_rank: 9
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
    value: 0.788
    std: 0.041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.08671'
    title: 'Permutation-Invariant graph partitioning: How graph neural networks capture
      structural interactions?'
    date: Dec 14, 2023
    date_display: Dec 2023
    date_iso: '2023-12-14'
    venue: Neural Networks
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 38
    sort_value: 0.788
    sort_std: 0.041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TopKPool
    model_key: topkpool
    model_plain: TopKPool
    value: 0.7768
    std: null
    paper_value: 0.7768
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
    source_ref: gao_2019_icml
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 68
    paper_rank: 68
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7048
    std: null
    paper_value: 0.7048
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
    source_ref: hamilton_2017_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.746
    at_pub_std: null
    at_pub_source_arxiv: '1904.13107'
    at_pub_source_title: Graph Convolutional Networks with EigenPooling
    at_pub_source_date_iso: '2019-04-30'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.041200000000000014
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7667
    true_std: 0.0305
    value_gap_source_arxiv: '2402.16346'
    value_gap_source_title: Boosting Graph Pooling with Persistent Homology
    value_gap_source_is_current_paper: false
    value_gap: 0.061900000000000066
    has_value_note: false
    value_note: ''
    sort_value: 0.7667
    sort_std: 0.0305
    global_rank: 113
    paper_rank: 499
    rank_delta: 386
    rank_delta_abs: 386
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Convolutional Networks with EigenPooling
    comparison_source_arxiv: '1904.13107'
    is_best: false
    is_std_outlier: false
  - model: ShortestPath
    model_key: shortestpath
    model_plain: ShortestPath
    value: 0.7643
    std: null
    paper_value: 0.7643
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: borgwardt_2005_icdm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7643
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7643
    sort_std: null
    global_rank: 135
    paper_rank: 135
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
    value: 0.76
    std: 0.032
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 170
    sort_value: 0.76
    sort_std: 0.032
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SortPool
    model_key: sortpool
    model_plain: SortPool
    value: 0.7554
    std: null
    paper_value: 0.7554
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
    source_ref: morris_2019_aaai
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.7391
    at_pub_std: 0.0072
    at_pub_source_arxiv: '1911.07979'
    at_pub_source_title: 'ASAP: Adaptive Structure Aware Pooling for Learning Hierarchical
      Graph Representations'
    at_pub_source_date_iso: '2019-11-18'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.01629999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7598
    true_std: 0.0176
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.0044000000000000705
    has_value_note: false
    value_note: ''
    sort_value: 0.7598
    sort_std: 0.0176
    global_rank: 173
    paper_rank: 215
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'ASAP: Adaptive Structure Aware Pooling for Learning
      Hierarchical Graph Representations'
    comparison_source_arxiv: '1911.07979'
    is_best: false
    is_std_outlier: false
  - model: SAGPool
    model_key: sagpool
    model_plain: SAGPool
    value: 0.7186
    std: null
    paper_value: 0.7186
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
    source_ref: lee_2019_icml
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.7186
    at_pub_std: 0.0097
    at_pub_source_arxiv: '1909.11855'
    at_pub_source_title: Universal Graph Transformer Self-Attention Networks
    at_pub_source_date_iso: '2019-09-26'
    at_pub_source_date_label: WWW 2019
    value_gap_source_date_iso: '2022-05-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7595
    true_std: 0.0452
    value_gap_source_arxiv: '2205.15068'
    value_gap_source_title: Embedding Graphs on Grassmann Manifold
    value_gap_source_is_current_paper: false
    value_gap: 0.040899999999999936
    has_value_note: false
    value_note: ''
    sort_value: 0.7595
    sort_std: 0.0452
    global_rank: 175
    paper_rank: 459
    rank_delta: 284
    rank_delta_abs: 284
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.75
    std: null
    paper_value: 0.75
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
    source_ref: niepert_2016_icml
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.759
    true_std: 0.028
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: false
    value_gap: 0.009000000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.759
    sort_std: 0.028
    global_rank: 177
    paper_rank: 275
    rank_delta: 98
    rank_delta_abs: 98
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.7376
    std: null
    paper_value: 0.7376
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
    source_ref: shervashidze_2011_jmlr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.756
    at_pub_std: 0.004
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2016-06-03'
    value_gap_source_date_label: NeurIPS 2016
    gap_vs_at_pub: 0.018399999999999972
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.756
    true_std: 0.004
    value_gap_source_arxiv: '1606.01141'
    value_gap_source_title: On Valid Optimal Assignment Kernels and Applications to
      Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.018399999999999972
    has_value_note: false
    value_note: ''
    sort_value: 0.756
    sort_std: 0.004
    global_rank: 208
    paper_rank: 362
    rank_delta: 154
    rank_delta_abs: 154
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Valid Optimal Assignment Kernels and Applications
      to Graph Classification
    comparison_source_arxiv: '1606.01141'
    is_best: false
    is_std_outlier: false
  - model: Sparse HGC
    model_key: sparse hgc
    model_plain: Sparse HGC
    value: 0.7546
    std: null
    paper_value: 0.7546
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
    source_ref: cangea_2018_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7546
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7546
    sort_std: null
    global_rank: 223
    paper_rank: 223
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL Optimal
    model_key: wl optimal
    model_plain: WL Optimal
    value: 0.7526
    std: null
    paper_value: 0.7526
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kriege_2016_nips
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7526
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7526
    sort_std: null
    global_rank: 253
    paper_rank: 253
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Set2Set
    model_key: set2set
    model_plain: Set2Set
    value: 0.7429
    std: null
    paper_value: 0.7429
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
    source_ref: vinyals_2015_iclr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.736
    at_pub_std: 0.037
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.006900000000000017
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7429
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7429
    sort_std: null
    global_rank: 336
    paper_rank: 336
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.7291
    std: null
    paper_value: 0.7291
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
    source_ref: shervashidze_2009_ais
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7291
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7291
    sort_std: null
    global_rank: 411
    paper_rank: 411
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ECC
    model_key: ecc
    model_plain: ECC
    value: 0.7265
    std: null
    paper_value: 0.7265
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
    source_ref: simonovsky_2017_cvpr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7265
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7265
    sort_std: null
    global_rank: 422
    paper_rank: 422
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CliquePool
    model_key: cliquepool
    model_plain: CliquePool
    value: 0.7259
    std: null
    paper_value: 0.7259
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
    source_ref: Luzhnica_2019_iclr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation mean accuracy
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-16'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7259
    true_std: null
    value_gap_source_arxiv: '2012.08734'
    value_gap_source_title: Hierarchical Graph Capsule Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7259
    sort_std: null
    global_rank: 426
    paper_rank: 426
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
- &id004
  dataset: Tox21
  rows:
  - model: HIMP
    model_key: himp
    model_plain: HIMP
    value: 0.874
    std: 0.005
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.874
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GINE w/ VN
    model_key: gine w/ vn
    model_plain: GINE w/ VN
    value: 0.872
    std: 0.003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.872
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: NaiveGINe+ K=3 w/ VN
    model_key: naivegine+ k=3 w/ vn
    model_plain: NaiveGINe+ K=3 w/ VN
    value: 0.87
    std: 0.004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.87
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.829
    std: 0.006
    paper_value: 0.829
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.7481
    at_pub_std: null
    at_pub_source_arxiv: '1801.03226'
    at_pub_source_title: Adaptive Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2018-01-10'
    at_pub_source_date_label: AAAI 2018
    value_gap_source_date_iso: '2020-11-30'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.08089999999999997
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.84
    true_std: 0.004
    value_gap_source_arxiv: '2011.15069'
    value_gap_source_title: Graph convolutions that can finally model local structure
    value_gap_source_is_current_paper: false
    value_gap: 0.01100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.84
    sort_std: 0.004
    global_rank: 14
    paper_rank: 23
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Adaptive Graph Convolutional Neural Networks
    comparison_source_arxiv: '1801.03226'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.829
    std: 0.0069
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1905.11577'
    title: Towards Interpretable Sparse Graph Representation Learning with Laplacian
      Pooling
    date: May 28, 2019
    date_display: May 2019
    date_iso: '2019-05-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 24
    sort_value: 0.829
    sort_std: 0.0069
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.828
    std: 0.004
    paper_value: 0.828
    paper_std: 0.004
    metric: ROC-AUC
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
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.828
    true_std: 0.004
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.828
    sort_std: 0.004
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Kernel SVM
    model_key: kernel svm
    model_plain: Kernel SVM
    value: 0.822
    std: 0.006
    paper_value: 0.822
    paper_std: 0.006
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.822
    true_std: 0.006
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.006
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
  - model: Weave
    model_key: weave
    model_plain: Weave
    value: 0.82
    std: 0.01
    paper_value: 0.82
    paper_std: 0.01
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
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.82
    true_std: 0.01
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.82
    sort_std: 0.01
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Bypass
    model_key: bypass
    model_plain: Bypass
    value: 0.81
    std: 0.013
    paper_value: 0.81
    paper_std: 0.013
    metric: ROC-AUC
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.81
    true_std: 0.013
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.81
    sort_std: 0.013
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Multitask
    model_key: multitask
    model_plain: Multitask
    value: 0.803
    std: 0.012
    paper_value: 0.803
    paper_std: 0.012
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
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.803
    true_std: 0.012
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.803
    sort_std: 0.012
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
  - model: IRV
    model_key: irv
    model_plain: IRV
    value: 0.799
    std: 0.006
    paper_value: 0.799
    paper_std: 0.006
    metric: ROC-AUC
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.799
    true_std: 0.006
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.799
    sort_std: 0.006
    global_rank: 63
    paper_rank: 63
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Logistic Regression
    model_key: logistic regression
    model_plain: Logistic Regression
    value: 0.794
    std: 0.015
    paper_value: 0.794
    paper_std: 0.015
    metric: ROC-AUC
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
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.794
    true_std: 0.015
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.794
    sort_std: 0.015
    global_rank: 76
    paper_rank: 76
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: XGBoost
    model_key: xgboost
    model_plain: XGBoost
    value: 0.794
    std: 0.014
    paper_value: 0.794
    paper_std: 0.014
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.794
    true_std: 0.014
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.794
    sort_std: 0.014
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
  - model: Random Forest
    model_key: random forest
    model_plain: Random Forest
    value: 0.769
    std: 0.015
    paper_value: 0.769
    paper_std: 0.015
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wu2018moleculenet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test split results for Tox21 graph classification
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.769
    true_std: 0.015
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.769
    sort_std: 0.015
    global_rank: 155
    paper_rank: 155
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
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
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
  - *id003
- benchmark: MoleculeNet
  datasets:
  - *id004
  - *id005
  - *id006
  - *id007
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: PROTEINS
      dataset_slug: proteins
    - dataset: COLLAB
      dataset_slug: collab
    - dataset: ENZYMES
      dataset_slug: enzymes
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: Tox21
      dataset_slug: tox21
    - dataset: BACE
      dataset_slug: bace
    - dataset: ESOL
      dataset_slug: esol
    - dataset: Lipophilicity
      dataset_slug: lipophilicity
main_figure: /figures/2002.09518/main_figure.jpegoptim.jpg
---

