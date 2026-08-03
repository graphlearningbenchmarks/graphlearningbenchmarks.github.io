---
title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D Graph Encoder'
arxiv_id: '2510.07289'
source_url: ''
authors:
- name: Xingtong Yu
  orcid: null
  s2_author_id: '2204706384'
  s2_url: null
- name: Chang Zhou
  orcid: null
  s2_author_id: '2271793882'
  s2_url: null
- name: Xinming Zhang
  orcid: null
  s2_author_id: '2268427703'
  s2_url: null
- name: Yuan Fang
  orcid: null
  s2_author_id: '2256784066'
  s2_url: null
published_date: Oct 8, 2025
published_date_iso: '2025-10-08'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Molecular graph representation learning is widely used in chemical and biomedical
  research. While pre-trained 2D graph encoders have demonstrated strong performance,
  they overlook the rich molecular domain knowledge associated with submolecular instances
  (atoms and bonds). While molecular pre-training approaches incorporate such knowledge
  into their pre-training objectives, they typically employ designs tailored to a
  specific type of knowledge, lacking the flexibility to integrate diverse knowledge
  present in molecules. Hence, reusing widely available and well-validated pre-trained
  2D encoders, while incorporating molecular domain knowledge during downstream adaptation,
  offers a more practical alternative. In this work, we propose MolGA, which adapts
  pre-trained 2D graph encoders to downstream molecular applications by flexibly incorporating
  diverse molecular domain knowledge. First, we propose a molecular alignment strategy
  that bridge the gap between pre-trained topological representations with domain-knowledge
  representations. Second, we introduce a conditional adaptation mechanism that generates
  instance-specific tokens to enable fine-grained integration of molecular domain
  knowledge for downstream tasks. Finally, we conduct extensive experiments on eleven
  public datasets, demonstrating the effectiveness of MolGA.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MolGA
mrr: 0.0071
adjusted_mrr: 0.0071
mrr_dataset_count: 7
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 7
  total: 9
task_categories:
- graph_classification
- graph_regression
experiment_scopes:
- graph-level
results:
- &id002
  dataset: BACE
  rows:
  - model: UnifiedMolPretrain
    model_key: protomol
    model_plain: UnifiedMolPretrain
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
  - model: UnifiedMolPretrain
    model_key: mmsg
    model_plain: UnifiedMolPretrain
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
  - model: UnifiedMolPretrain
    model_key: memgnn
    model_plain: UnifiedMolPretrain
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5021
    std: 0.0555
    paper_value: 0.5021
    paper_std: 0.0555
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D adaptation on BACE
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86
    at_pub_std: 0.011
    at_pub_source_arxiv: '2006.04804'
    at_pub_source_title: Optimal Transport Graph Neural Networks
    at_pub_source_date_iso: '2020-06-08'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-08'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.3579
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.86
    true_std: 0.011
    value_gap_source_arxiv: '2006.04804'
    value_gap_source_title: Optimal Transport Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.3579
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.011
    global_rank: 47
    paper_rank: 328
    rank_delta: 281
    rank_delta_abs: 281
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Optimal Transport Graph Neural Networks
    comparison_source_arxiv: '2006.04804'
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.5807
    std: 0.0924
    paper_value: 0.5807
    paper_std: 0.0924
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.856
    at_pub_std: 0.011
    at_pub_source_arxiv: '2407.12136'
    at_pub_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    at_pub_source_date_iso: '2024-07-16'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.2753
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.856
    true_std: 0.011
    value_gap_source_arxiv: '2604.16586'
    value_gap_source_title: A Systematic Survey and Benchmark of Deep Learning for
      Molecular Property Prediction in the Foundation Model Era
    value_gap_source_is_current_paper: false
    value_gap: 0.2753
    has_value_note: false
    value_note: ''
    sort_value: 0.856
    sort_std: 0.011
    global_rank: 55
    paper_rank: 313
    rank_delta: 258
    rank_delta_abs: 258
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    comparison_source_arxiv: '2407.12136'
    is_best: false
    is_std_outlier: false
  - model: MoleBlend
    model_key: moleblend
    model_plain: MoleBlend
    value: 0.5717
    std: 0.0819
    paper_value: 0.5717
    paper_std: 0.0819
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.837
    at_pub_std: 0.014
    at_pub_source_arxiv: '2405.10343'
    at_pub_source_title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view
      Molecular Representation Learning'
    at_pub_source_date_iso: '2024-05-15'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-05-15'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.2653
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.837
    true_std: 0.014
    value_gap_source_arxiv: '2405.10343'
    value_gap_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.2653
    has_value_note: false
    value_note: ''
    sort_value: 0.837
    sort_std: 0.014
    global_rank: 89
    paper_rank: 313
    rank_delta: 224
    rank_delta_abs: 224
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    comparison_source_arxiv: '2405.10343'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5053
    std: 0.062
    paper_value: 0.5053
    paper_std: 0.062
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D adaptation on BACE
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.823
    at_pub_std: 0.034
    at_pub_source_arxiv: '2407.12136'
    at_pub_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    at_pub_source_date_iso: '2024-07-16'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.3177
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.823
    true_std: 0.034
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.3177
    has_value_note: false
    value_note: ''
    sort_value: 0.823
    sort_std: 0.034
    global_rank: 117
    paper_rank: 327
    rank_delta: 210
    rank_delta_abs: 210
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    comparison_source_arxiv: '2407.12136'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.5546
    std: 0.061
    paper_value: 0.5546
    paper_std: 0.061
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
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
    gap_vs_at_pub: 0.2574000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.812
    true_std: null
    value_gap_source_arxiv: '2404.11568'
    value_gap_source_title: On the Scalability of GNNs for Molecular Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.2574000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.812
    sort_std: null
    global_rank: 142
    paper_rank: 315
    rank_delta: 173
    rank_delta_abs: 173
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unified 2D and 3D Pre-Training of Molecular Representations
    comparison_source_arxiv: '2207.08806'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.522
    std: 0.0619
    paper_value: 0.522
    paper_std: 0.0619
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.782
    at_pub_std: 0.012
    at_pub_source_arxiv: '2205.15746'
    at_pub_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    at_pub_source_date_iso: '2022-05-31'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.26
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.782
    true_std: 0.012
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.26
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.012
    global_rank: 210
    paper_rank: 324
    rank_delta: 114
    rank_delta_abs: 114
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    comparison_source_arxiv: '2205.15746'
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 0.5243
    std: 0.0362
    paper_value: 0.5243
    paper_std: 0.0362
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.677
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2209.15240'
    at_pub_source_title: Universal Prompt Tuning for Graph Neural Networks
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.15270000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.677
    true_std: 0.0126
    value_gap_source_arxiv: '2209.15240'
    value_gap_source_title: Universal Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.15270000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.677
    sort_std: 0.0126
    global_rank: 293
    paper_rank: 324
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Universal Prompt Tuning for Graph Neural Networks
    comparison_source_arxiv: '2209.15240'
    is_best: false
    is_std_outlier: false
  - model: MolGA
    model_key: molga
    model_plain: MolGA
    value: 0.5494
    std: 0.0537
    paper_value: 0.5494
    paper_std: 0.0537
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D+Mol adaptation
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5494
    true_std: 0.0537
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5494
    sort_std: 0.0537
    global_rank: 316
    paper_rank: 316
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComENet
    model_key: comenet
    model_plain: ComENet
    value: 0.5457
    std: 0.1021
    paper_value: 0.5457
    paper_std: 0.1021
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on BACE
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5457
    true_std: 0.1021
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5457
    sort_std: 0.1021
    global_rank: 317
    paper_rank: 317
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 0.5443
    std: 0.1341
    paper_value: 0.5443
    paper_std: 0.1341
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on BACE
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5443
    true_std: 0.1341
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5443
    sort_std: 0.1341
    global_rank: 318
    paper_rank: 318
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.5406
    std: 0.13
    paper_value: 0.5406
    paper_std: 0.13
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on BACE
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5406
    true_std: 0.13
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5406
    sort_std: 0.13
    global_rank: 320
    paper_rank: 320
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
  dataset: BBBP
  rows:
  - model: UnifiedMolPretrain
    model_key: cams-llama
    model_plain: UnifiedMolPretrain
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
    global_rank: 1
    sort_value: 0.942
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UnifiedMolPretrain
    model_key: se(3)-i mpph
    model_plain: UnifiedMolPretrain
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
    global_rank: 2
    sort_value: 0.94
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UnifiedMolPretrain
    model_key: masking node + supervised
    model_plain: UnifiedMolPretrain
    value: 0.9343
    std: 0.025
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.06010'
    title: Does GNN Pretraining Help Molecular Representation?
    date: Jul 13, 2022
    date_display: Jul 2022
    date_iso: '2022-07-13'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9343
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.6461
    std: 0.1224
    paper_value: 0.6461
    paper_std: 0.1224
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.887
    at_pub_std: 0.019
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.2409
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.887
    true_std: 0.019
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.2409
    has_value_note: false
    value_note: ''
    sort_value: 0.887
    sort_std: 0.019
    global_rank: 27
    paper_rank: 275
    rank_delta: 248
    rank_delta_abs: 248
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6623
    std: 0.1383
    paper_value: 0.6623
    paper_std: 0.1383
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D adaptation on BBBP
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.881
    at_pub_std: 0.036
    at_pub_source_arxiv: '2208.04529'
    at_pub_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    at_pub_source_date_iso: '2022-08-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-08-09'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.2187
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.881
    true_std: 0.036
    value_gap_source_arxiv: '2208.04529'
    value_gap_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    value_gap_source_is_current_paper: false
    value_gap: 0.2187
    has_value_note: false
    value_note: ''
    sort_value: 0.881
    sort_std: 0.036
    global_rank: 29
    paper_rank: 248
    rank_delta: 219
    rank_delta_abs: 219
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
    value: 0.6905
    std: 0.08
    paper_value: 0.6905
    paper_std: 0.08
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
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
    gap_vs_at_pub: 0.16949999999999998
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
    value_gap: 0.16949999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.034
    global_rank: 40
    paper_rank: 180
    rank_delta: 140
    rank_delta_abs: 140
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: MoleBlend
    model_key: moleblend
    model_plain: MoleBlend
    value: 0.7145
    std: 0.0945
    paper_value: 0.7145
    paper_std: 0.0945
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.73
    at_pub_std: 0.008
    at_pub_source_arxiv: '2405.10343'
    at_pub_source_title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view
      Molecular Representation Learning'
    at_pub_source_date_iso: '2024-05-15'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-05-15'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.015499999999999958
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.73
    true_std: 0.008
    value_gap_source_arxiv: '2405.10343'
    value_gap_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.015499999999999958
    has_value_note: false
    value_note: ''
    sort_value: 0.73
    sort_std: 0.008
    global_rank: 81
    paper_rank: 114
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.7178
    std: 0.078
    paper_value: 0.7178
    paper_std: 0.078
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.724
    at_pub_std: 0.004
    at_pub_source_arxiv: '2407.12136'
    at_pub_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    at_pub_source_date_iso: '2024-07-16'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.006199999999999983
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.724
    true_std: 0.004
    value_gap_source_arxiv: '2604.16586'
    value_gap_source_title: A Systematic Survey and Benchmark of Deep Learning for
      Molecular Property Prediction in the Foundation Model Era
    value_gap_source_is_current_paper: false
    value_gap: 0.006199999999999983
    has_value_note: false
    value_note: ''
    sort_value: 0.724
    sort_std: 0.004
    global_rank: 92
    paper_rank: 106
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolGA
    model_key: molga
    model_plain: MolGA
    value: 0.7197
    std: 0.1234
    paper_value: 0.7197
    paper_std: 0.1234
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D+Mol adaptation
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7197
    true_std: 0.1234
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7197
    sort_std: 0.1234
    global_rank: 105
    paper_rank: 105
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 0.6888
    std: 0.1103
    paper_value: 0.6888
    paper_std: 0.1103
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6929
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2209.15240'
    at_pub_source_title: Universal Prompt Tuning for Graph Neural Networks
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.0040999999999999925
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6929
    true_std: 0.0019
    value_gap_source_arxiv: '2209.15240'
    value_gap_source_title: Universal Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0040999999999999925
    has_value_note: false
    value_note: ''
    sort_value: 0.6929
    sort_std: 0.0019
    global_rank: 174
    paper_rank: 187
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5972
    std: 0.1242
    paper_value: 0.5972
    paper_std: 0.1242
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D adaptation on BBBP
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6776
    at_pub_std: null
    at_pub_source_arxiv: '2211.03666'
    at_pub_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    at_pub_source_date_iso: '2022-11-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08040000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6776
    true_std: null
    value_gap_source_arxiv: '2211.03666'
    value_gap_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    value_gap_source_is_current_paper: false
    value_gap: 0.08040000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.6776
    sort_std: null
    global_rank: 209
    paper_rank: 312
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComENet
    model_key: comenet
    model_plain: ComENet
    value: 0.6689
    std: 0.0994
    paper_value: 0.6689
    paper_std: 0.0994
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on BBBP
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6689
    true_std: 0.0994
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6689
    sort_std: 0.0994
    global_rank: 237
    paper_rank: 237
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.6641
    std: 0.1043
    paper_value: 0.6641
    paper_std: 0.1043
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on BBBP
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6641
    true_std: 0.1043
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6641
    sort_std: 0.1043
    global_rank: 244
    paper_rank: 244
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 0.6554
    std: 0.1051
    paper_value: 0.6554
    paper_std: 0.1051
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on BBBP
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6554
    true_std: 0.1051
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6554
    sort_std: 0.1051
    global_rank: 264
    paper_rank: 264
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
  dataset: ClinTox
  rows:
  - model: UnifiedMolPretrain
    model_key: se(3)-i mpph
    model_plain: UnifiedMolPretrain
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
  - model: UnifiedMolPretrain
    model_key: ka-gcn
    model_plain: UnifiedMolPretrain
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
  - model: UnifiedMolPretrain
    model_key: ka-gat
    model_plain: UnifiedMolPretrain
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5459
    std: 0.0533
    paper_value: 0.5459
    paper_std: 0.0533
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task using 2D topology
      adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.913
    at_pub_std: 0.017
    at_pub_source_arxiv: '2112.03806'
    at_pub_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
    at_pub_source_date_iso: '2021-12-07'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-12-07'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.3671
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.913
    true_std: 0.017
    value_gap_source_arxiv: '2112.03806'
    value_gap_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural
      Network'
    value_gap_source_is_current_paper: false
    value_gap: 0.3671
    has_value_note: false
    value_note: ''
    sort_value: 0.913
    sort_std: 0.017
    global_rank: 20
    paper_rank: 260
    rank_delta: 240
    rank_delta_abs: 240
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural
      Network'
    comparison_source_arxiv: '2112.03806'
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.6232
    std: 0.0731
    paper_value: 0.6232
    paper_std: 0.0731
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task (reference
      only, uses 2D+Mol pre-training and adaptation).
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.901
    true_std: 0.013
    value_gap_source_arxiv: '2604.16586'
    value_gap_source_title: A Systematic Survey and Benchmark of Deep Learning for
      Molecular Property Prediction in the Foundation Model Era
    value_gap_source_is_current_paper: false
    value_gap: 0.27780000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.901
    sort_std: 0.013
    global_rank: 27
    paper_rank: 228
    rank_delta: 201
    rank_delta_abs: 201
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoleBlend
    model_key: moleblend
    model_plain: MoleBlend
    value: 0.6056
    std: 0.0636
    paper_value: 0.6056
    paper_std: 0.0636
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task (reference
      only, uses 2D+Mol pre-training and adaptation).
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.876
    at_pub_std: 0.007
    at_pub_source_arxiv: '2405.10343'
    at_pub_source_title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view
      Molecular Representation Learning'
    at_pub_source_date_iso: '2024-05-15'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-05-15'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.2704
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.876
    true_std: 0.007
    value_gap_source_arxiv: '2405.10343'
    value_gap_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.2704
    has_value_note: false
    value_note: ''
    sort_value: 0.876
    sort_std: 0.007
    global_rank: 48
    paper_rank: 232
    rank_delta: 184
    rank_delta_abs: 184
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    comparison_source_arxiv: '2405.10343'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.5743
    std: 0.0612
    paper_value: 0.5743
    paper_std: 0.0612
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task (reference
      only, uses 2D+Mol pre-training and adaptation).
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
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
    gap_vs_at_pub: 0.29069999999999996
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
    value_gap: 0.29069999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.865
    sort_std: 0.017
    global_rank: 54
    paper_rank: 249
    rank_delta: 195
    rank_delta_abs: 195
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Group Symmetric Stochastic Differential Equation Model
      for Molecule Multi-modal Pretraining
    comparison_source_arxiv: '2305.18407'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5291
    std: 0.0457
    paper_value: 0.5291
    paper_std: 0.0457
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task using 2D topology
      adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.826
    at_pub_std: 0.045
    at_pub_source_arxiv: '2305.15745'
    at_pub_source_title: Robust Ante-hoc Graph Explainer using Bilevel Optimization
    at_pub_source_date_iso: '2023-05-25'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-05-25'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.29689999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.826
    true_std: 0.045
    value_gap_source_arxiv: '2305.15745'
    value_gap_source_title: Robust Ante-hoc Graph Explainer using Bilevel Optimization
    value_gap_source_is_current_paper: false
    value_gap: 0.29689999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.826
    sort_std: 0.045
    global_rank: 73
    paper_rank: 262
    rank_delta: 189
    rank_delta_abs: 189
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Robust Ante-hoc Graph Explainer using Bilevel Optimization
    comparison_source_arxiv: '2305.15745'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.5558
    std: 0.0684
    paper_value: 0.5558
    paper_std: 0.0684
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task using 2D pre-training
      and 2D adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.789
    at_pub_std: 0.042
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.23320000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.789
    true_std: 0.042
    value_gap_source_arxiv: '2110.07728'
    value_gap_source_title: 16 Pre-training Molecular Graph Representation with 3D
      Geometry
    value_gap_source_is_current_paper: false
    value_gap: 0.23320000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.042
    global_rank: 107
    paper_rank: 259
    rank_delta: 152
    rank_delta_abs: 152
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 16 Pre-training Molecular Graph Representation with 3D
      Geometry
    comparison_source_arxiv: '2110.07728'
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.5425
    std: 0.1054
    paper_value: 0.5425
    paper_std: 0.1054
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task using 2D+Mol
      adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.76
    at_pub_std: null
    at_pub_source_arxiv: '2109.11730'
    at_pub_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    at_pub_source_date_iso: '2021-09-24'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-09-24'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.21750000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.76
    true_std: null
    value_gap_source_arxiv: '2109.11730'
    value_gap_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.21750000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: null
    global_rank: 132
    paper_rank: 260
    rank_delta: 128
    rank_delta_abs: 128
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    comparison_source_arxiv: '2109.11730'
    is_best: false
    is_std_outlier: false
  - model: MolGA
    model_key: molga
    model_plain: MolGA
    value: 0.5731
    std: 0.0687
    paper_value: 0.5731
    paper_std: 0.0687
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task using 2D pre-training
      and 2D+Mol adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5731
    true_std: 0.0687
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5731
    sort_std: 0.0687
    global_rank: 250
    paper_rank: 250
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComENet
    model_key: comenet
    model_plain: ComENet
    value: 0.5589
    std: 0.0909
    paper_value: 0.5589
    paper_std: 0.0909
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task using 2D+Mol
      adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5589
    true_std: 0.0909
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5589
    sort_std: 0.0909
    global_rank: 255
    paper_rank: 255
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 0.5567
    std: 0.0708
    paper_value: 0.5567
    paper_std: 0.0708
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task using 2D pre-training
      and 2D adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5537
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2209.15240'
    at_pub_source_title: Universal Prompt Tuning for Graph Neural Networks
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5567
    true_std: 0.0708
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5567
    sort_std: 0.0708
    global_rank: 258
    paper_rank: 258
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 0.5383
    std: 0.1087
    paper_value: 0.5383
    paper_std: 0.1087
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC evaluation on molecular classification task using 2D+Mol
      adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5383
    true_std: 0.1087
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5383
    sort_std: 0.1087
    global_rank: 261
    paper_rank: 261
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
  dataset: ESOL
  rows:
  - model: KCL
    model_key: mat
    model_plain: KCL
    value: 0.278
    std: 0.02
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2002.08264'
    title: Molecule Attention Transformer
    date: Feb 19, 2020
    date_display: Feb 2020
    date_iso: '2020-02-19'
    venue: Graph Representation Learning workshop and Machine Learning and the Physical
      Sciences workshop at NeurIPS 2019
    codebase_url: https://github.com/gmum/MAT
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.278
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: KCL
    model_key: smiles
    model_plain: KCL
    value: 0.356
    std: 0.017
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2002.08264'
    title: Molecule Attention Transformer
    date: Feb 19, 2020
    date_display: Feb 2020
    date_iso: '2020-02-19'
    venue: Graph Representation Learning workshop and Machine Learning and the Physical
      Sciences workshop at NeurIPS 2019
    codebase_url: https://github.com/gmum/MAT
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.356
    sort_std: 0.017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KCL
    model_key: conan-fgw
    model_plain: KCL
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
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 2.377
    std: 0.078
    paper_value: 2.377
    paper_std: 0.078
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D+Mol adaptation on ESOL
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.633
    at_pub_std: null
    at_pub_source_arxiv: '2106.09553'
    at_pub_source_title: How Much Structural Information Large Scale Molecular Language
      Representations Can Capture?
    at_pub_source_date_iso: '2021-06-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-09-24'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 1.7439999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.633
    true_std: null
    value_gap_source_arxiv: '2109.11730'
    value_gap_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 1.7439999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.633
    sort_std: null
    global_rank: 19
    paper_rank: 126
    rank_delta: 107
    rank_delta_abs: 107
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    comparison_source_arxiv: '2106.09553'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 2.635
    std: 0.116
    paper_value: 2.635
    paper_std: 0.116
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D adaptation on ESOL
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.552
    at_pub_std: 0.007
    at_pub_source_arxiv: '2305.13987'
    at_pub_source_title: On Structural Expressive Power of Graph Transformers
    at_pub_source_date_iso: '2023-05-23'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2020-06-08'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 2.0829999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.654
    true_std: 0.028
    value_gap_source_arxiv: '2006.04804'
    value_gap_source_title: Optimal Transport Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 1.9809999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.654
    sort_std: 0.028
    global_rank: 23
    paper_rank: 126
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Structural Expressive Power of Graph Transformers
    comparison_source_arxiv: '2305.13987'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 2.764
    std: 0.122
    paper_value: 2.764
    paper_std: 0.122
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D adaptation on ESOL
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.564
    at_pub_std: 0.015
    at_pub_source_arxiv: '2305.13987'
    at_pub_source_title: On Structural Expressive Power of Graph Transformers
    at_pub_source_date_iso: '2023-05-23'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 2.1999999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.876
    true_std: 0.037
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 1.888
    has_value_note: false
    value_note: ''
    sort_value: 0.876
    sort_std: 0.037
    global_rank: 47
    paper_rank: 126
    rank_delta: 79
    rank_delta_abs: 79
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Structural Expressive Power of Graph Transformers
    comparison_source_arxiv: '2305.13987'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 2.038
    std: 0.047
    paper_value: 2.038
    paper_std: 0.047
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.959
    at_pub_std: 0.047
    at_pub_source_arxiv: '2110.04126'
    at_pub_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    at_pub_source_date_iso: '2021-10-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: 1.0789999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.959
    true_std: 0.047
    value_gap_source_arxiv: '2110.04126'
    value_gap_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 1.0789999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.959
    sort_std: 0.047
    global_rank: 60
    paper_rank: 118
    rank_delta: 58
    rank_delta_abs: 58
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    comparison_source_arxiv: '2110.04126'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 2.257
    std: 0.043
    paper_value: 2.257
    paper_std: 0.043
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.091
    at_pub_std: 0.021
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 1.1660000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 1.091
    true_std: 0.021
    value_gap_source_arxiv: '2209.15101'
    value_gap_source_title: Improving Molecular Pretraining with Complementary Featurizations
    value_gap_source_is_current_paper: false
    value_gap: 1.1660000000000001
    has_value_note: false
    value_note: ''
    sort_value: 1.091
    sort_std: 0.021
    global_rank: 79
    paper_rank: 122
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 16 Pre-training Molecular Graph Representation with 3D
      Geometry
    comparison_source_arxiv: '2110.07728'
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 1.175
    std: 0.02
    paper_value: 1.175
    paper_std: 0.02
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.798
    at_pub_std: null
    at_pub_source_arxiv: '2106.09553'
    at_pub_source_title: How Much Structural Information Large Scale Molecular Language
      Representations Can Capture?
    at_pub_source_date_iso: '2021-06-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.377
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.175
    true_std: 0.02
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.175
    sort_std: 0.02
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    comparison_source_arxiv: '2106.09553'
    is_best: false
    is_std_outlier: false
  - model: MoleBlend
    model_key: moleblend
    model_plain: MoleBlend
    value: 1.496
    std: 0.032
    paper_value: 1.496
    paper_std: 0.032
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.496
    true_std: 0.032
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.496
    sort_std: 0.032
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolGA
    model_key: molga
    model_plain: MolGA
    value: 1.973
    std: 0.043
    paper_value: 1.973
    paper_std: 0.043
    metric: RMSE
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D+Mol adaptation
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.973
    true_std: 0.043
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.973
    sort_std: 0.043
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 2.052
    std: 0.045
    paper_value: 2.052
    paper_std: 0.045
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.052
    true_std: 0.045
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.052
    sort_std: 0.045
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
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 2.135
    std: 0.151
    paper_value: 2.135
    paper_std: 0.151
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D+Mol adaptation on ESOL
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.135
    true_std: 0.151
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.135
    sort_std: 0.151
    global_rank: 120
    paper_rank: 120
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComENet
    model_key: comenet
    model_plain: ComENet
    value: 2.317
    std: 0.21
    paper_value: 2.317
    paper_std: 0.21
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D+Mol adaptation on ESOL
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.317
    true_std: 0.21
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.317
    sort_std: 0.21
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
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id006
  dataset: FreeSolv
  rows:
  - model: D&D-Node +vn
    model_key: se(3)-i mpph
    model_plain: D&D-Node +vn
    value: 0.354
    std: 0.053
    metric: RMSE
    higher_is_better: false
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
    sort_value: 0.354
    sort_std: 0.053
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: ecfp-4 + rf
    model_plain: D&D-Node +vn
    value: 0.56
    std: 0.066
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
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
    feature_source_evidence: trained on ECFP-4 fingerprints
    is_global_top: true
    global_rank: 2
    sort_value: 0.56
    sort_std: 0.066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: geomgcl
    model_plain: D&D-Node +vn
    value: 0.866
    std: null
    metric: RMSE
    higher_is_better: false
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
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: The model uses a 2D-3D geometric contrastive scheme to
      bridge knowledge between 2D chemical semantics and 3D spatial information.
    is_global_top: true
    global_rank: 3
    sort_value: 0.866
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 4.049
    std: 0.213
    paper_value: 4.049
    paper_std: 0.213
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on FreeSolv
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.978
    at_pub_std: null
    at_pub_source_arxiv: '2106.09553'
    at_pub_source_title: How Much Structural Information Large Scale Molecular Language
      Representations Can Capture?
    at_pub_source_date_iso: '2021-06-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-09-24'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 3.0710000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.978
    true_std: null
    value_gap_source_arxiv: '2109.11730'
    value_gap_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 3.0710000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.978
    sort_std: null
    global_rank: 6
    paper_rank: 116
    rank_delta: 110
    rank_delta_abs: 110
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    comparison_source_arxiv: '2106.09553'
    is_best: false
    is_std_outlier: false
  - model: MoleBlend
    model_key: moleblend
    model_plain: MoleBlend
    value: 1.851
    std: 0.068
    paper_value: 1.851
    paper_std: 0.068
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.851
    true_std: 0.068
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.851
    sort_std: 0.068
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 1.957
    std: 0.073
    paper_value: 1.957
    paper_std: 0.073
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.877
    at_pub_std: null
    at_pub_source_arxiv: '2106.09553'
    at_pub_source_title: How Much Structural Information Large Scale Molecular Language
      Representations Can Capture?
    at_pub_source_date_iso: '2021-06-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.08000000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.957
    true_std: 0.073
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.957
    sort_std: 0.073
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    comparison_source_arxiv: '2106.09553'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 4.267
    std: 0.203
    paper_value: 4.267
    paper_std: 0.203
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D adaptation on FreeSolv
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.0072
    at_pub_std: 0.141
    at_pub_source_arxiv: '2311.04837'
    at_pub_source_title: Identifying Semantic Component for Robust Molecular Property
      Prediction
    at_pub_source_date_iso: '2023-11-08'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-11-08'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 2.2598000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 2.0072
    true_std: 0.141
    value_gap_source_arxiv: '2311.04837'
    value_gap_source_title: Identifying Semantic Component for Robust Molecular Property
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 2.2598000000000003
    has_value_note: false
    value_note: ''
    sort_value: 2.0072
    sort_std: 0.141
    global_rank: 40
    paper_rank: 120
    rank_delta: 80
    rank_delta_abs: 80
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Identifying Semantic Component for Robust Molecular Property
      Prediction
    comparison_source_arxiv: '2311.04837'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 4.298
    std: 0.143
    paper_value: 4.298
    paper_std: 0.143
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D adaptation on FreeSolv
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.1519
    at_pub_std: 0.0645
    at_pub_source_arxiv: '2311.04837'
    at_pub_source_title: Identifying Semantic Component for Robust Molecular Property
      Prediction
    at_pub_source_date_iso: '2023-11-08'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-11-08'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 2.1461
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 2.1519
    true_std: 0.0645
    value_gap_source_arxiv: '2311.04837'
    value_gap_source_title: Identifying Semantic Component for Robust Molecular Property
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 2.1461
    has_value_note: false
    value_note: ''
    sort_value: 2.1519
    sort_std: 0.0645
    global_rank: 48
    paper_rank: 121
    rank_delta: 73
    rank_delta_abs: 73
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Identifying Semantic Component for Robust Molecular Property
      Prediction
    comparison_source_arxiv: '2311.04837'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 2.767
    std: 0.033
    paper_value: 2.767
    paper_std: 0.033
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.767
    true_std: 0.033
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.767
    sort_std: 0.033
    global_rank: 82
    paper_rank: 82
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 4.612
    std: 0.133
    paper_value: 4.612
    paper_std: 0.133
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation on FreeSolv
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 3.166
    at_pub_std: 0.027
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 1.4460000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 3.166
    true_std: 0.027
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 1.4460000000000002
    has_value_note: false
    value_note: ''
    sort_value: 3.166
    sort_std: 0.027
    global_rank: 99
    paper_rank: 124
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    comparison_source_arxiv: '2412.15589'
    is_best: false
    is_std_outlier: false
  - model: MolGA
    model_key: molga
    model_plain: MolGA
    value: 3.602
    std: 0.131
    paper_value: 3.602
    paper_std: 0.131
    metric: RMSE
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on FreeSolv
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.602
    true_std: 0.131
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.602
    sort_std: 0.131
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
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 3.9
    std: 0.138
    paper_value: 3.9
    paper_std: 0.138
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on FreeSolv
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.9
    true_std: 0.138
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.9
    sort_std: 0.138
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComENet
    model_key: comenet
    model_plain: ComENet
    value: 4.049
    std: 0.285
    paper_value: 4.049
    paper_std: 0.285
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on FreeSolv
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 4.049
    true_std: 0.285
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 4.049
    sort_std: 0.285
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 4.517
    std: 0.129
    paper_value: 4.517
    paper_std: 0.129
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation on FreeSolv
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 4.517
    true_std: 0.129
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 4.517
    sort_std: 0.129
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
  - model: SE(3)-I MPPH
    model_key: memgnn
    model_plain: SE(3)-I MPPH
    value: 0.556
    std: 0.023
    metric: RMSE
    higher_is_better: false
    is_baseline: true
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
    global_rank: 1
    sort_value: 0.556
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SE(3)-I MPPH
    model_key: protos-l2
    model_plain: SE(3)-I MPPH
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
  - model: SE(3)-I MPPH
    model_key: protow-l2
    model_plain: SE(3)-I MPPH
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
    value: 1.466
    std: 0.131
    paper_value: 1.466
    paper_std: 0.131
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D adaptation for molecular property prediction.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.655
    at_pub_std: 0.036
    at_pub_source_arxiv: '2002.09518'
    at_pub_source_title: Memory-Based Graph Networks
    at_pub_source_date_iso: '2020-02-21'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.8109999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.655
    true_std: 0.036
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.8109999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.655
    sort_std: 0.036
    global_rank: 6
    paper_rank: 94
    rank_delta: 88
    rank_delta_abs: 88
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Memory-Based Graph Networks
    comparison_source_arxiv: '2002.09518'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 1.249
    std: 0.014
    paper_value: 1.249
    paper_std: 0.014
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D pre-training followed by 2D adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.714
    at_pub_std: 0.011
    at_pub_source_arxiv: '2312.07633'
    at_pub_source_title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    at_pub_source_date_iso: '2023-12-12'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.5350000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.714
    true_std: 0.011
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.5350000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.714
    sort_std: 0.011
    global_rank: 18
    paper_rank: 89
    rank_delta: 71
    rank_delta_abs: 71
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    comparison_source_arxiv: '2312.07633'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.945
    std: 0.014
    paper_value: 0.945
    paper_std: 0.014
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (for reference).
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.718
    at_pub_std: 0.016
    at_pub_source_arxiv: '2209.15101'
    at_pub_source_title: Improving Molecular Pretraining with Complementary Featurizations
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.22699999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.718
    true_std: 0.016
    value_gap_source_arxiv: '2209.15101'
    value_gap_source_title: Improving Molecular Pretraining with Complementary Featurizations
    value_gap_source_is_current_paper: false
    value_gap: 0.22699999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.718
    sort_std: 0.016
    global_rank: 22
    paper_rank: 74
    rank_delta: 52
    rank_delta_abs: 52
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Molecular Pretraining with Complementary Featurizations
    comparison_source_arxiv: '2209.15101'
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 1.379
    std: 0.133
    paper_value: 1.379
    paper_std: 0.133
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D+Mol adaptation for molecular property prediction.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.614
    at_pub_std: null
    at_pub_source_arxiv: '2106.09553'
    at_pub_source_title: How Much Structural Information Large Scale Molecular Language
      Representations Can Capture?
    at_pub_source_date_iso: '2021-06-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-09-24'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.765
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.742
    true_std: null
    value_gap_source_arxiv: '2109.11730'
    value_gap_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.637
    has_value_note: false
    value_note: ''
    sort_value: 0.742
    sort_std: null
    global_rank: 33
    paper_rank: 94
    rank_delta: 61
    rank_delta_abs: 61
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    comparison_source_arxiv: '2106.09553'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 1.445
    std: 0.068
    paper_value: 1.445
    paper_std: 0.068
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D adaptation for molecular property prediction.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.753
    at_pub_std: null
    at_pub_source_arxiv: '2211.03666'
    at_pub_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    at_pub_source_date_iso: '2022-11-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.6920000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.753
    true_std: null
    value_gap_source_arxiv: '2211.03666'
    value_gap_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    value_gap_source_is_current_paper: false
    value_gap: 0.6920000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.753
    sort_std: null
    global_rank: 36
    paper_rank: 94
    rank_delta: 58
    rank_delta_abs: 58
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    comparison_source_arxiv: '2211.03666'
    is_best: false
    is_std_outlier: false
  - model: MoleBlend
    model_key: moleblend
    model_plain: MoleBlend
    value: 0.774
    std: 0.012
    paper_value: 0.774
    paper_std: 0.012
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (for reference).
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.774
    true_std: 0.012
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.774
    sort_std: 0.012
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.84
    std: 0.22
    paper_value: 0.84
    paper_std: 0.22
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (for reference).
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.66
    at_pub_std: null
    at_pub_source_arxiv: '2106.09553'
    at_pub_source_title: How Much Structural Information Large Scale Molecular Language
      Representations Can Capture?
    at_pub_source_date_iso: '2021-06-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.17999999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.84
    true_std: 0.22
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.84
    sort_std: 0.22
    global_rank: 59
    paper_rank: 59
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: MolGA
    model_key: molga
    model_plain: MolGA
    value: 1.187
    std: 0.015
    paper_value: 1.187
    paper_std: 0.015
    metric: RMSE
    higher_is_better: false
    is_baseline: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D pre-training followed by 2D+Mol adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.187
    true_std: 0.015
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.187
    sort_std: 0.015
    global_rank: 88
    paper_rank: 88
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 1.242
    std: 0.017
    paper_value: 1.242
    paper_std: 0.017
    metric: RMSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: 2D pre-training followed by 2D adaptation.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.242
    true_std: 0.017
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.242
    sort_std: 0.017
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
  - model: ComENet
    model_key: comenet
    model_plain: ComENet
    value: 1.309
    std: 0.048
    paper_value: 1.309
    paper_std: 0.048
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D+Mol adaptation for molecular property prediction.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.309
    true_std: 0.048
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.309
    sort_std: 0.048
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
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 1.335
    std: 0.127
    paper_value: 1.335
    paper_std: 0.127
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard 2D+Mol adaptation for molecular property prediction.
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.335
    true_std: 0.127
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.335
    sort_std: 0.127
    global_rank: 92
    paper_rank: 92
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
- &id004
  dataset: SIDER
  rows:
  - model: UnifiedMolPretrain
    model_key: ka-gat
    model_plain: UnifiedMolPretrain
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
  - model: UnifiedMolPretrain
    model_key: ka-gcn
    model_plain: UnifiedMolPretrain
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
  - model: UnifiedMolPretrain
    model_key: graphkan
    model_plain: UnifiedMolPretrain
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
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.5417
    std: 0.063
    paper_value: 0.5417
    paper_std: 0.063
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.672
    true_std: 0.004
    value_gap_source_arxiv: '2604.16586'
    value_gap_source_title: A Systematic Survey and Benchmark of Deep Learning for
      Molecular Property Prediction in the Foundation Model Era
    value_gap_source_is_current_paper: false
    value_gap: 0.13030000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.672
    sort_std: 0.004
    global_rank: 18
    paper_rank: 230
    rank_delta: 212
    rank_delta_abs: 212
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoleBlend
    model_key: moleblend
    model_plain: MoleBlend
    value: 0.5285
    std: 0.0425
    paper_value: 0.5285
    paper_std: 0.0425
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.649
    at_pub_std: 0.003
    at_pub_source_arxiv: '2405.10343'
    at_pub_source_title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view
      Molecular Representation Learning'
    at_pub_source_date_iso: '2024-05-15'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-05-15'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.12050000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.649
    true_std: 0.003
    value_gap_source_arxiv: '2405.10343'
    value_gap_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.12050000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.649
    sort_std: 0.003
    global_rank: 51
    paper_rank: 232
    rank_delta: 181
    rank_delta_abs: 181
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    comparison_source_arxiv: '2405.10343'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.5082
    std: 0.0419
    paper_value: 0.5082
    paper_std: 0.0419
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Molecular graph pre-training (reference only)
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
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
    gap_vs_at_pub: 0.13080000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.639
    true_std: null
    value_gap_source_arxiv: '2404.11568'
    value_gap_source_title: On the Scalability of GNNs for Molecular Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.13080000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.639
    sort_std: null
    global_rank: 72
    paper_rank: 234
    rank_delta: 162
    rank_delta_abs: 162
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unified 2D and 3D Pre-Training of Molecular Representations
    comparison_source_arxiv: '2207.08806'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.5159
    std: 0.0445
    paper_value: 0.5159
    paper_std: 0.0445
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation on SIDER
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6183
    at_pub_std: 0.006
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.10239999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6183
    true_std: 0.006
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.10239999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6183
    sort_std: 0.006
    global_rank: 115
    paper_rank: 234
    rank_delta: 119
    rank_delta_abs: 119
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    comparison_source_arxiv: '2412.15589'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5243
    std: 0.053
    paper_value: 0.5243
    paper_std: 0.053
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D adaptation on SIDER
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.615
    at_pub_std: 0.025
    at_pub_source_arxiv: '2208.04529'
    at_pub_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    at_pub_source_date_iso: '2022-08-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-08-09'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0907
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.615
    true_std: 0.025
    value_gap_source_arxiv: '2208.04529'
    value_gap_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    value_gap_source_is_current_paper: false
    value_gap: 0.0907
    has_value_note: false
    value_note: ''
    sort_value: 0.615
    sort_std: 0.025
    global_rank: 126
    paper_rank: 234
    rank_delta: 108
    rank_delta_abs: 108
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    comparison_source_arxiv: '2208.04529'
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.5085
    std: 0.0483
    paper_value: 0.5085
    paper_std: 0.0483
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on SIDER
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.615
    at_pub_std: null
    at_pub_source_arxiv: '2109.11730'
    at_pub_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    at_pub_source_date_iso: '2021-09-24'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-09-24'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.10650000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.615
    true_std: null
    value_gap_source_arxiv: '2109.11730'
    value_gap_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.10650000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.615
    sort_std: null
    global_rank: 127
    paper_rank: 234
    rank_delta: 107
    rank_delta_abs: 107
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    comparison_source_arxiv: '2109.11730'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5084
    std: 0.055
    paper_value: 0.5084
    paper_std: 0.055
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D adaptation on SIDER
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6085
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2311.04837'
    at_pub_source_title: Identifying Semantic Component for Robust Molecular Property
      Prediction
    at_pub_source_date_iso: '2023-11-08'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-11-08'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.10010000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6085
    true_std: 0.0043
    value_gap_source_arxiv: '2311.04837'
    value_gap_source_title: Identifying Semantic Component for Robust Molecular Property
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.10010000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.6085
    sort_std: 0.0043
    global_rank: 153
    paper_rank: 234
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Identifying Semantic Component for Robust Molecular Property
      Prediction
    comparison_source_arxiv: '2311.04837'
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 0.5153
    std: 0.042
    paper_value: 0.5153
    paper_std: 0.042
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D adaptation on SIDER
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5871
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2209.15240'
    at_pub_source_title: Universal Prompt Tuning for Graph Neural Networks
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.07179999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5871
    true_std: 0.0013
    value_gap_source_arxiv: '2209.15240'
    value_gap_source_title: Universal Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07179999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.5871
    sort_std: 0.0013
    global_rank: 204
    paper_rank: 234
    rank_delta: 30
    rank_delta_abs: 30
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Universal Prompt Tuning for Graph Neural Networks
    comparison_source_arxiv: '2209.15240'
    is_best: false
    is_std_outlier: false
  - model: MolGA
    model_key: molga
    model_plain: MolGA
    value: 0.5261
    std: 0.0542
    paper_value: 0.5261
    paper_std: 0.0542
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D pre-training and 2D+Mol adaptation on SIDER
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5261
    true_std: 0.0542
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5261
    sort_std: 0.0542
    global_rank: 233
    paper_rank: 233
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: ComENet
    model_key: comenet
    model_plain: ComENet
    value: 0.5052
    std: 0.0622
    paper_value: 0.5052
    paper_std: 0.0622
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on SIDER
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5052
    true_std: 0.0622
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5052
    sort_std: 0.0622
    global_rank: 235
    paper_rank: 235
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 0.5026
    std: 0.0592
    paper_value: 0.5026
    paper_std: 0.0592
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2D+Mol adaptation on SIDER
    date: Oct 8, 2025
    date_display: Oct 2025
    date_iso: '2025-10-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5026
    true_std: 0.0592
    value_gap_source_arxiv: '2510.07289'
    value_gap_source_title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D
      Graph Encoder'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5026
    sort_std: 0.0592
    global_rank: 236
    paper_rank: 236
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
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
  - *id007
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: BBBP
      dataset_slug: bbbp
    - dataset: BACE
      dataset_slug: bace
    - dataset: ClinTox
      dataset_slug: clintox
    - dataset: SIDER
      dataset_slug: sider
    - dataset: ESOL
      dataset_slug: esol
    - dataset: FreeSolv
      dataset_slug: freesolv
    - dataset: Lipophilicity
      dataset_slug: lipophilicity
single_proposed_model: MolGA
---

