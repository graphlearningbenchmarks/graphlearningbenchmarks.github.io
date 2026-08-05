---
title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent Molecular Property
  Prediction: A Systematic Survey'
arxiv_id: '2402.07249'
source_url: ''
authors:
- name: Taojie Kuang
  orcid: null
  s2_author_id: '2232608353'
  s2_url: null
- name: Pengfei Liu
  orcid: null
  s2_author_id: '2283185054'
  s2_url: null
- name: Zhixiang Ren
  orcid: null
  s2_author_id: '2283123678'
  s2_url: null
published_date: Feb 11, 2024
published_date_iso: '2024-02-11'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'The precise prediction of molecular properties is essential for advancements
  in drug development, particularly in virtual screening and compound optimization.
  The recent introduction of numerous deep learning-based methods has shown remarkable
  potential in enhancing molecular property prediction (MPP), especially improving
  accuracy and insights into molecular structures. Yet, two critical questions arise:
  does the integration of domain knowledge augment the accuracy of molecular property
  prediction and does employing multi-modal data fusion yield more precise results
  than unique data source methods? To explore these matters, we comprehensively review
  and quantitatively analyze recent deep learning methods based on various benchmarks.
  We discover that integrating molecular information significantly improves molecular
  property prediction (MPP) for both regression and classification tasks. Specifically,
  regression improvements, measured by reductions in root mean square error (RMSE),
  are up to 4.0\ We also discover that enriching 2D graphs with 1D SMILES boosts multi-modal
  learning performance for regression tasks by up to 9.1\ The two consolidated insights
  offer crucial guidance for future advancements in drug discovery.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 6
  total: 9
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: BACE
  rows:
  - model: MAGPrompt+
    model_key: protomol
    model_plain: MAGPrompt+
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
  - model: MAGPrompt+
    model_key: mmsg
    model_plain: MAGPrompt+
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
  - model: MAGPrompt+
    model_key: memgnn
    model_plain: MAGPrompt+
    value: 0.907
    std: 0.0
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.907
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.726
    std: null
    paper_value: 0.726
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
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
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BACE task using standard split
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.861
    at_pub_std: 0.013
    at_pub_source_arxiv: '2006.04804'
    at_pub_source_title: Optimal Transport Graph Neural Networks
    at_pub_source_date_iso: '2020-06-08'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.135
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8646
    true_std: 0.0081
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.13860000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8646
    sort_std: 0.0081
    global_rank: 41
    paper_rank: 254
    rank_delta: 213
    rank_delta_abs: 213
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Optimal Transport Graph Neural Networks
    comparison_source_arxiv: '2006.04804'
    is_best: false
    is_std_outlier: false
  - model: MolLM
    model_key: mollm
    model_plain: MolLM
    value: 0.841
    std: null
    paper_value: 0.841
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: tang2023mollm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BACE task using standard split
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.841
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.841
    sort_std: null
    global_rank: 84
    paper_rank: 84
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolFM
    model_key: molfm
    model_plain: MolFM
    value: 0.839
    std: null
    paper_value: 0.839
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: luo2023molfm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BACE task using standard split
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.839
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.839
    sort_std: null
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
  - model: MoleculeSTM
    model_key: moleculestm
    model_plain: MoleculeSTM
    value: 0.82
    std: null
    paper_value: 0.82
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2023multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BACE task using standard split
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.82
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.82
    sort_std: null
    global_rank: 125
    paper_rank: 125
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.812
    std: null
    paper_value: 0.812
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2021pre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BACE task using standard split
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.812
    at_pub_std: 0.009
    at_pub_source_arxiv: '2207.08806'
    at_pub_source_title: Unified 2D and 3D Pre-Training of Molecular Representations
    at_pub_source_date_iso: '2022-07-14'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-04-17'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.812
    true_std: null
    value_gap_source_arxiv: '2404.11568'
    value_gap_source_title: On the Scalability of GNNs for Molecular Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.812
    sort_std: null
    global_rank: 141
    paper_rank: 141
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIT-Mol
    model_key: git-mol
    model_plain: GIT-Mol
    value: 0.811
    std: null
    paper_value: 0.811
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2024git
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BACE task using standard split
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.811
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: null
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KV-PLM
    model_key: kv-plm
    model_plain: KV-PLM
    value: 0.785
    std: null
    paper_value: 0.785
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zeng2022deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BACE task using standard split
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.785
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.785
    sort_std: null
    global_rank: 203
    paper_rank: 203
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-K
    model_key: momu-k
    model_plain: MoMu-K
    value: 0.771
    std: null
    paper_value: 0.771
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BACE task using standard split
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.771
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.771
    sort_std: null
    global_rank: 222
    paper_rank: 222
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-S
    model_key: momu-s
    model_plain: MoMu-S
    value: 0.767
    std: null
    paper_value: 0.767
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BACE task using standard split
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.767
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.767
    sort_std: null
    global_rank: 227
    paper_rank: 227
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
- &id003
  dataset: BBBP
  rows:
  - model: MAGPrompt+
    model_key: magprompt+
    model_plain: MAGPrompt+
    value: 0.9432
    std: 0.0238
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.05567'
    title: 'MAGPrompt: Message-Adaptive Graph Prompt Tuning for Graph Neural Networks'
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9432
    sort_std: 0.0238
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MAGPrompt+
    model_key: cams-llama
    model_plain: MAGPrompt+
    value: 0.942
    std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 100.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2601.02530'
    title: 'Multi-scale Graph Autoregressive Modeling: Molecular Property Prediction
      via Next Token Prediction'
    date: Jan 5, 2026
    date_display: Jan 2026
    date_iso: '2026-01-05'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.942
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MAGPrompt+
    model_key: se(3)-i mpph
    model_plain: MAGPrompt+
    value: 0.94
    std: 0.021
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_display: Dec 2023
    date_iso: '2023-12-12'
    venue: NeurIPS 2023 AI for Science Workshop
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: integrating SE(3)-invariance into Vietoris-Rips persistent
      homology
    is_global_top: true
    global_rank: 3
    sort_value: 0.94
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.654
    std: null
    paper_value: 0.654
    paper_std: null
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
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BBBP task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.873
    at_pub_std: 0.036
    at_pub_source_arxiv: '2208.04529'
    at_pub_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    at_pub_source_date_iso: '2022-08-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.21899999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8875
    true_std: 0.0049
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.23349999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8875
    sort_std: 0.0049
    global_rank: 32
    paper_rank: 257
    rank_delta: 225
    rank_delta_abs: 225
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    comparison_source_arxiv: '2208.04529'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.724
    std: null
    paper_value: 0.724
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2021pre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BBBP task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86
    at_pub_std: 0.034
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.136
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.86
    true_std: 0.034
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.136
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.034
    global_rank: 47
    paper_rank: 86
    rank_delta: 39
    rank_delta_abs: 39
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: MolLM
    model_key: mollm
    model_plain: MolLM
    value: 0.757
    std: null
    paper_value: 0.757
    paper_std: null
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
    table_ref: Table 1
    source_ref: tang2023mollm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BBBP task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.757
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.757
    sort_std: null
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
  - model: GIT-Mol
    model_key: git-mol
    model_plain: GIT-Mol
    value: 0.739
    std: null
    paper_value: 0.739
    paper_std: null
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
    table_ref: Table 1
    source_ref: liu2024git
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BBBP task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.739
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.739
    sort_std: null
    global_rank: 70
    paper_rank: 70
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolFM
    model_key: molfm
    model_plain: MolFM
    value: 0.729
    std: null
    paper_value: 0.729
    paper_std: null
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
    table_ref: Table 1
    source_ref: luo2023molfm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BBBP task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.729
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: null
    global_rank: 79
    paper_rank: 79
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KV-PLM
    model_key: kv-plm
    model_plain: KV-PLM
    value: 0.72
    std: null
    paper_value: 0.72
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zeng2022deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BBBP task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.72
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.72
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
  - model: MoleculeSTM
    model_key: moleculestm
    model_plain: MoleculeSTM
    value: 0.708
    std: null
    paper_value: 0.708
    paper_std: null
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
    table_ref: Table 1
    source_ref: liu2023multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BBBP task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.708
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.708
    sort_std: null
    global_rank: 119
    paper_rank: 119
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-S
    model_key: momu-s
    model_plain: MoMu-S
    value: 0.705
    std: null
    paper_value: 0.705
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BBBP task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.705
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.705
    sort_std: null
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
  - model: MoMu-K
    model_key: momu-k
    model_plain: MoMu-K
    value: 0.701
    std: null
    paper_value: 0.701
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet BBBP task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.701
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.701
    sort_std: null
    global_rank: 137
    paper_rank: 137
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
- &id004
  dataset: ClinTox
  rows:
  - model: EdgePrompt+
    model_key: se(3)-i mpph
    model_plain: EdgePrompt+
    value: 0.993
    std: 0.004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_display: Dec 2023
    date_iso: '2023-12-12'
    venue: NeurIPS 2023 AI for Science Workshop
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: integrating SE(3)-invariance into Vietoris-Rips persistent
      homology
    is_global_top: true
    global_rank: 1
    sort_value: 0.993
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: ka-gcn
    model_plain: EdgePrompt+
    value: 0.992
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
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.992
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: ka-gat
    model_plain: EdgePrompt+
    value: 0.991
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
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.991
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MoleculeSTM
    model_key: moleculestm
    model_plain: MoleculeSTM
    value: 0.925
    std: null
    paper_value: 0.925
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2023multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet ClinTox classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.925
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.925
    sort_std: null
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolLM
    model_key: mollm
    model_plain: MolLM
    value: 0.911
    std: null
    paper_value: 0.911
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: tang2023mollm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet ClinTox classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.911
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.911
    sort_std: null
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
  - model: KV-PLM
    model_key: kv-plm
    model_plain: KV-PLM
    value: 0.892
    std: null
    paper_value: 0.892
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zeng2022deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet ClinTox classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.892
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.892
    sort_std: null
    global_rank: 31
    paper_rank: 31
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIT-Mol
    model_key: git-mol
    model_plain: GIT-Mol
    value: 0.883
    std: null
    paper_value: 0.883
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2024git
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet ClinTox classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.883
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.883
    sort_std: null
    global_rank: 35
    paper_rank: 35
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
    value: 0.588
    std: null
    paper_value: 0.588
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
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
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet ClinTox classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.881
    at_pub_std: 0.025
    at_pub_source_arxiv: '2112.03806'
    at_pub_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
    at_pub_source_date_iso: '2021-12-07'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-12-07'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.29300000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.881
    true_std: 0.025
    value_gap_source_arxiv: '2112.03806'
    value_gap_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural
      Network'
    value_gap_source_is_current_paper: false
    value_gap: 0.29300000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.881
    sort_std: 0.025
    global_rank: 37
    paper_rank: 224
    rank_delta: 187
    rank_delta_abs: 187
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural
      Network'
    comparison_source_arxiv: '2112.03806'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.79
    std: null
    paper_value: 0.79
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2021pre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet ClinTox classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.865
    at_pub_std: 0.017
    at_pub_source_arxiv: '2305.18407'
    at_pub_source_title: A Group Symmetric Stochastic Differential Equation Model
      for Molecule Multi-modal Pretraining
    at_pub_source_date_iso: '2023-05-28'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-09'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.07499999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.865
    true_std: 0.017
    value_gap_source_arxiv: '2405.05665'
    value_gap_source_title: 'SubGDiff: A Subgraph Diffusion Model to Improve Molecular
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07499999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.865
    sort_std: 0.017
    global_rank: 49
    paper_rank: 93
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Group Symmetric Stochastic Differential Equation Model
      for Molecule Multi-modal Pretraining
    comparison_source_arxiv: '2305.18407'
    is_best: false
    is_std_outlier: false
  - model: MoMu-S
    model_key: momu-s
    model_plain: MoMu-S
    value: 0.799
    std: null
    paper_value: 0.799
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet ClinTox classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.799
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.799
    sort_std: null
    global_rank: 89
    paper_rank: 89
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolFM
    model_key: molfm
    model_plain: MolFM
    value: 0.797
    std: null
    paper_value: 0.797
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: luo2023molfm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet ClinTox classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.797
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.797
    sort_std: null
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-K
    model_key: momu-k
    model_plain: MoMu-K
    value: 0.774
    std: null
    paper_value: 0.774
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet ClinTox classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.774
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.774
    sort_std: null
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
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: SIDER
  rows:
  - model: DGI
    model_key: ka-gat
    model_plain: DGI
    value: 0.847
    std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.847
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DGI
    model_key: ka-gcn
    model_plain: DGI
    value: 0.842
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.842
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: graphkan
    model_plain: DGI
    value: 0.837
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.837
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolLM
    model_key: mollm
    model_plain: MolLM
    value: 0.71
    std: null
    paper_value: 0.71
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: tang2023mollm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet SIDER task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.71
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.71
    sort_std: null
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolFM
    model_key: molfm
    model_plain: MolFM
    value: 0.642
    std: null
    paper_value: 0.642
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: luo2023molfm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet SIDER task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.642
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.642
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.58
    std: null
    paper_value: 0.58
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
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
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet SIDER task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.616
    at_pub_std: 0.025
    at_pub_source_arxiv: '2208.04529'
    at_pub_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    at_pub_source_date_iso: '2022-08-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.03600000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6403
    true_std: 0.0104
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.06030000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6403
    sort_std: 0.0104
    global_rank: 66
    paper_rank: 213
    rank_delta: 147
    rank_delta_abs: 147
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    comparison_source_arxiv: '2208.04529'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.639
    std: null
    paper_value: 0.639
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2021pre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet SIDER task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.639
    at_pub_std: 0.012
    at_pub_source_arxiv: '2207.08806'
    at_pub_source_title: Unified 2D and 3D Pre-Training of Molecular Representations
    at_pub_source_date_iso: '2022-07-14'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-04-17'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.639
    true_std: null
    value_gap_source_arxiv: '2404.11568'
    value_gap_source_title: On the Scalability of GNNs for Molecular Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.639
    sort_std: null
    global_rank: 70
    paper_rank: 70
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoleculeSTM
    model_key: moleculestm
    model_plain: MoleculeSTM
    value: 0.637
    std: null
    paper_value: 0.637
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2023multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet SIDER task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.637
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.637
    sort_std: null
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
  - model: GIT-Mol
    model_key: git-mol
    model_plain: GIT-Mol
    value: 0.634
    std: null
    paper_value: 0.634
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2024git
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet SIDER task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.634
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.634
    sort_std: null
    global_rank: 78
    paper_rank: 78
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-S
    model_key: momu-s
    model_plain: MoMu-S
    value: 0.605
    std: null
    paper_value: 0.605
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet SIDER task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.605
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.605
    sort_std: null
    global_rank: 165
    paper_rank: 165
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-K
    model_key: momu-k
    model_plain: MoMu-K
    value: 0.604
    std: null
    paper_value: 0.604
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet SIDER task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.604
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.604
    sort_std: null
    global_rank: 172
    paper_rank: 172
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KV-PLM
    model_key: kv-plm
    model_plain: KV-PLM
    value: 0.598
    std: null
    paper_value: 0.598
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zeng2022deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet SIDER task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.598
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.598
    sort_std: null
    global_rank: 189
    paper_rank: 189
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
- &id001
  dataset: Tox21
  rows:
  - model: HOD-GNN
    model_key: himp
    model_plain: HOD-GNN
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
  - model: HOD-GNN
    model_key: gine w/ vn
    model_plain: HOD-GNN
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
  - model: HOD-GNN
    model_key: naivegine+ k=3 w/ vn
    model_plain: HOD-GNN
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.749
    std: null
    paper_value: 0.749
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
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
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet Tox21 classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.829
    at_pub_std: 0.0069
    at_pub_source_arxiv: '1905.11577'
    at_pub_source_title: Towards Interpretable Sparse Graph Representation Learning
      with Laplacian Pooling
    at_pub_source_date_iso: '2019-05-28'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-05-28'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.07999999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.829
    true_std: 0.0069
    value_gap_source_arxiv: '1905.11577'
    value_gap_source_title: Towards Interpretable Sparse Graph Representation Learning
      with Laplacian Pooling
    value_gap_source_is_current_paper: false
    value_gap: 0.07999999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: 0.0069
    global_rank: 25
    paper_rank: 230
    rank_delta: 205
    rank_delta_abs: 205
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Interpretable Sparse Graph Representation Learning
      with Laplacian Pooling
    comparison_source_arxiv: '1905.11577'
    is_best: false
    is_std_outlier: false
  - model: MolLM
    model_key: mollm
    model_plain: MolLM
    value: 0.8
    std: null
    paper_value: 0.8
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: tang2023mollm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet Tox21 classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: null
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.745
    std: null
    paper_value: 0.745
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2021pre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet Tox21 classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.799
    at_pub_std: 0.018
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.05400000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.799
    true_std: 0.018
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.05400000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.799
    sort_std: 0.018
    global_rank: 65
    paper_rank: 241
    rank_delta: 176
    rank_delta_abs: 176
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: MolFM
    model_key: molfm
    model_plain: MolFM
    value: 0.772
    std: null
    paper_value: 0.772
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: luo2023molfm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet Tox21 classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.772
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.772
    sort_std: null
    global_rank: 150
    paper_rank: 150
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoleculeSTM
    model_key: moleculestm
    model_plain: MoleculeSTM
    value: 0.769
    std: null
    paper_value: 0.769
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2023multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet Tox21 classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.769
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.769
    sort_std: null
    global_rank: 159
    paper_rank: 159
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIT-Mol
    model_key: git-mol
    model_plain: GIT-Mol
    value: 0.759
    std: null
    paper_value: 0.759
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2024git
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet Tox21 classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.759
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.759
    sort_std: null
    global_rank: 186
    paper_rank: 186
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-S
    model_key: momu-s
    model_plain: MoMu-S
    value: 0.756
    std: null
    paper_value: 0.756
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet Tox21 classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.756
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.756
    sort_std: null
    global_rank: 195
    paper_rank: 195
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-K
    model_key: momu-k
    model_plain: MoMu-K
    value: 0.756
    std: null
    paper_value: 0.756
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet Tox21 classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.756
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.756
    sort_std: null
    global_rank: 196
    paper_rank: 196
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KV-PLM
    model_key: kv-plm
    model_plain: KV-PLM
    value: 0.7
    std: null
    paper_value: 0.7
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zeng2022deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet Tox21 classification task
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7
    sort_std: null
    global_rank: 297
    paper_rank: 297
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
- &id006
  dataset: ToxCast
  rows:
  - model: GIN (Supervised EdgePred)
    model_key: geomgcl
    model_plain: GIN (Supervised EdgePred)
    value: 0.763
    std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_display: Sep 2021
    date_iso: '2021-09-24'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: The model uses 2D and 3D views derived from the molecule,
      which are standard geometric augmentations/views for this task.
    is_global_top: true
    global_rank: 1
    sort_value: 0.763
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN (Supervised EdgePred)
    model_key: light deepgpt
    model_plain: GIN (Supervised EdgePred)
    value: 0.757
    std: 0.011
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.37
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_display: Sep 2023
    date_iso: '2023-09-18'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.757
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN (Supervised EdgePred)
    model_key: d&d-node +vn
    model_plain: GIN (Supervised EdgePred)
    value: 0.7556
    std: 0.0068
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.04062'
    title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising
      and Cross-Modal Distillation'
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7556
    sort_std: 0.0068
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.616
    std: null
    paper_value: 0.616
    paper_std: null
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
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet classification task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.634
    at_pub_std: 0.007
    at_pub_source_arxiv: '2112.03806'
    at_pub_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
    at_pub_source_date_iso: '2021-12-07'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.018000000000000016
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7095
    true_std: 0.0027
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.09350000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7095
    sort_std: 0.0027
    global_rank: 38
    paper_rank: 185
    rank_delta: 147
    rank_delta_abs: 147
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural
      Network'
    comparison_source_arxiv: '2112.03806'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.631
    std: null
    paper_value: 0.631
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2021pre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet classification task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.689
    at_pub_std: 0.01
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.05799999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.689
    true_std: 0.01
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.05799999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.689
    sort_std: 0.01
    global_rank: 58
    paper_rank: 161
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: MolLM
    model_key: mollm
    model_plain: MolLM
    value: 0.682
    std: null
    paper_value: 0.682
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: tang2023mollm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet classification task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.682
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.682
    sort_std: null
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
  - model: GIT-Mol
    model_key: git-mol
    model_plain: GIT-Mol
    value: 0.668
    std: null
    paper_value: 0.668
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2024git
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet classification task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.668
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.668
    sort_std: null
    global_rank: 78
    paper_rank: 78
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoleculeSTM
    model_key: moleculestm
    model_plain: MoleculeSTM
    value: 0.652
    std: null
    paper_value: 0.652
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2023multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet classification task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.652
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.652
    sort_std: null
    global_rank: 112
    paper_rank: 112
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolFM
    model_key: molfm
    model_plain: MolFM
    value: 0.644
    std: null
    paper_value: 0.644
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: luo2023molfm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet classification task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.644
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.644
    sort_std: null
    global_rank: 125
    paper_rank: 125
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-S
    model_key: momu-s
    model_plain: MoMu-S
    value: 0.634
    std: null
    paper_value: 0.634
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet classification task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.634
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.634
    sort_std: null
    global_rank: 147
    paper_rank: 147
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoMu-K
    model_key: momu-k
    model_plain: MoMu-K
    value: 0.63
    std: null
    paper_value: 0.63
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: su2022molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet classification task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.63
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.63
    sort_std: null
    global_rank: 167
    paper_rank: 167
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KV-PLM
    model_key: kv-plm
    model_plain: KV-PLM
    value: 0.55
    std: null
    paper_value: 0.55
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zeng2022deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MoleculeNet classification task using ROC-AUC
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.55
    true_std: null
    value_gap_source_arxiv: '2402.07249'
    value_gap_source_title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent
      Molecular Property Prediction: A Systematic Survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.55
    sort_std: null
    global_rank: 208
    paper_rank: 208
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
- benchmark: MoleculeNet
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
  - *id005
  - *id006
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: Tox21
      dataset_slug: tox21
    - dataset: BACE
      dataset_slug: bace
    - dataset: BBBP
      dataset_slug: bbbp
    - dataset: ClinTox
      dataset_slug: clintox
    - dataset: SIDER
      dataset_slug: sider
    - dataset: ToxCast
      dataset_slug: toxcast
main_figure: /figures/2402.07249/main_figure.jpegoptim.jpg
---

