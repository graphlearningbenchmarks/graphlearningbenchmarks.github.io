---
title: Efficient Text-Attributed Graph Learning through Selective Annotation and Graph
  Alignment
arxiv_id: '2506.07168'
source_url: ''
authors:
- name: Huanyi Xie
  orcid: null
  s2_author_id: '2312101594'
  s2_url: null
- name: Lijie Hu
  orcid: null
  s2_author_id: '2153121378'
  s2_url: null
- name: Lu Yu
  orcid: null
  s2_author_id: '2284728569'
  s2_url: null
- name: Tianhao Huang
  orcid: null
  s2_author_id: '2294678140'
  s2_url: null
- name: Longfei Li
  orcid: null
  s2_author_id: '2310856464'
  s2_url: null
- name: Meng Li
  orcid: null
  s2_author_id: '2365956716'
  s2_url: null
- name: Jun Zhou
  orcid: null
  s2_author_id: '2238908467'
  s2_url: null
- name: Huan Wang
  orcid: null
  s2_author_id: '2197900527'
  s2_url: null
- name: Di Wang
  orcid: null
  s2_author_id: '2303281490'
  s2_url: null
published_date: Jun 8, 2025
published_date_iso: '2025-06-08'
published_venue: TMLR 2025
published_conference: TMLR 2025
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: In the realm of Text-attributed Graphs (TAGs), traditional graph neural
  networks (GNNs) often fall short due to the complex textual information associated
  with each node. Recent methods have improved node representations by leveraging
  large language models (LLMs) to enhance node text features, but these approaches
  typically require extensive annotations or fine-tuning across all nodes, which is
  both time-consuming and costly. To overcome these challenges, we introduce GAGA,
  an efficient framework for TAG representation learning. GAGA reduces annotation
  time and cost by focusing on annotating only representative nodes and edges. It
  constructs an annotation graph that captures the topological relationships among
  these annotations. Furthermore, GAGA employs a two-level alignment module to effectively
  integrate the annotation graph with the TAG, aligning their underlying structures.
  Experiments show that GAGA achieves classification accuracies on par with or surpassing
  state-of-the-art methods while requiring only 1\
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GAGA
mrr: 0.0372
adjusted_mrr: 0.0372
mrr_dataset_count: 3
benchmark_categories:
- Classic
- OGB
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Cora
  rows:
  - model: SGC+TSC
    model_key: exphormer
    model_plain: SGC+TSC
    value: 0.9635
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9635
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: sgformer
    model_plain: SGC+TSC
    value: 0.9629
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9629
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: coral
    model_plain: SGC+TSC
    value: 0.9574
    std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9574
    sort_std: 0.0039
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ENGINE
    model_key: engine
    model_plain: ENGINE
    value: 0.9148
    std: 0.001
    paper_value: 0.9148
    paper_std: 0.001
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9148
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9148
    true_std: 0.001
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9148
    sort_std: 0.001
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TAPE
    model_key: tape
    model_plain: TAPE
    value: 0.9119
    std: 0.0012
    paper_value: 0.9119
    paper_std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.893
    at_pub_std: null
    at_pub_source_arxiv: '2310.16421'
    at_pub_source_title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.018900000000000028
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9119
    true_std: 0.0012
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9119
    sort_std: 0.0012
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    comparison_source_arxiv: '2310.16421'
    is_best: false
    is_std_outlier: false
  - model: InstructGLM
    model_key: instructglm
    model_plain: InstructGLM
    value: 0.8708
    std: 0.0012
    paper_value: 0.8708
    paper_std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9077
    at_pub_std: null
    at_pub_source_arxiv: '2310.16421'
    at_pub_source_title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03689999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9077
    true_std: null
    value_gap_source_arxiv: '2310.16421'
    value_gap_source_title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.03689999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9077
    sort_std: null
    global_rank: 26
    paper_rank: 194
    rank_delta: 168
    rank_delta_abs: 168
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    comparison_source_arxiv: '2310.16421'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8824
    std: 0.001
    paper_value: 0.8824
    paper_std: 0.001
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.018000000000000016
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.018000000000000016
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 33
    paper_rank: 122
    rank_delta: 89
    rank_delta_abs: 89
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: GAGA
    model_key: gaga
    model_plain: GAGA
    value: 0.8967
    std: 0.0012
    paper_value: 0.8967
    paper_std: 0.0012
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8967
    true_std: 0.0012
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8967
    sort_std: 0.0012
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8911
    std: 0.0012
    paper_value: 0.8911
    paper_std: 0.0012
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8573
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.03380000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8911
    true_std: 0.0012
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8911
    sort_std: 0.0012
    global_rank: 65
    paper_rank: 65
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    comparison_source_arxiv: '2401.15569'
    is_best: false
    is_std_outlier: false
  - model: RevGAT
    model_key: revgat
    model_plain: RevGAT
    value: 0.8911
    std: 0.001
    paper_value: 0.8911
    paper_std: 0.001
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8911
    at_pub_std: 0.0
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8911
    true_std: 0.0
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8911
    sort_std: 0.0
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimTEG
    model_key: simteg
    model_plain: SimTEG
    value: 0.8804
    std: 0.0012
    paper_value: 0.8804
    paper_std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8804
    at_pub_std: 0.0136
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8804
    true_std: 0.0012
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8804
    sort_std: 0.0012
    global_rank: 130
    paper_rank: 130
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLEM
    model_key: glem
    model_plain: GLEM
    value: 0.7469
    std: 0.0018
    paper_value: 0.7469
    paper_std: 0.0018
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.856
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2024-01-28'
    value_gap_source_date_label: IJCAI 2024
    gap_vs_at_pub: 0.10909999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.856
    true_std: 0.0009
    value_gap_source_arxiv: '2401.15569'
    value_gap_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.10909999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.856
    sort_std: 0.0009
    global_rank: 284
    paper_rank: 888
    rank_delta: 604
    rank_delta_abs: 604
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    comparison_source_arxiv: '2401.15569'
    is_best: false
    is_std_outlier: false
  - model: GIANT
    model_key: giant
    model_plain: GIANT
    value: 0.8552
    std: 0.0018
    paper_value: 0.8552
    paper_std: 0.0018
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8552
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8552
    true_std: 0.0018
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8552
    sort_std: 0.0018
    global_rank: 287
    paper_rank: 287
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.8041
    std: 0.002
    paper_value: 0.8041
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8041
    at_pub_std: 0.003
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8041
    true_std: 0.003
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8041
    sort_std: 0.003
    global_rank: 759
    paper_rank: 759
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
    value: 0.6388
    std: 0.0012
    paper_value: 0.6388
    paper_std: 0.0012
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7768
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.138
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.138
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 840
    paper_rank: 981
    rank_delta: 141
    rank_delta_abs: 141
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
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
- &id002
  dataset: PubMed
  rows:
  - model: R-SoftGraphAIN
    model_key: lgtl
    model_plain: R-SoftGraphAIN
    value: 0.9518
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9518
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: sagn
    model_plain: R-SoftGraphAIN
    value: 0.9517
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.24867'
    title: 'Clustering as Reasoning: A $k$-Means Interpretation of Chain-of-Thought
      Graph Learning'
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    venue: Accepted by ICML 2026
    codebase_url: https://github.com/Uncnbb/KCoT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9517
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: mixhop (lo)
    model_plain: R-SoftGraphAIN
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAGA
    model_key: gaga
    model_plain: GAGA
    value: 0.9462
    std: 0.002
    paper_value: 0.9462
    paper_std: 0.002
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9462
    true_std: 0.002
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9462
    sort_std: 0.002
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
  - model: TAPE
    model_key: tape
    model_plain: TAPE
    value: 0.9431
    std: 0.0015
    paper_value: 0.9431
    paper_std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9431
    true_std: 0.0015
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9431
    sort_std: 0.0015
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
  - model: InstructGLM
    model_key: instructglm
    model_plain: InstructGLM
    value: 0.9384
    std: 0.0015
    paper_value: 0.9384
    paper_std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9384
    true_std: 0.0015
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9384
    sort_std: 0.0015
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8031
    std: 0.0015
    paper_value: 0.8031
    paper_std: 0.0015
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9296
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.12649999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9296
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.12649999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: null
    global_rank: 21
    paper_rank: 441
    rank_delta: 420
    rank_delta_abs: 420
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: false
    is_std_outlier: false
  - model: GLEM
    model_key: glem
    model_plain: GLEM
    value: 0.9257
    std: 0.002
    paper_value: 0.9257
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9257
    true_std: 0.002
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9257
    sort_std: 0.002
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8881
    std: 0.0015
    paper_value: 0.8881
    paper_std: 0.0015
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7844
    at_pub_std: null
    at_pub_source_arxiv: '2310.14527'
    at_pub_source_title: 'Marginal Nodes Matter: Towards Structure Fairness in Graphs'
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.10370000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8881
    true_std: 0.0015
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8881
    sort_std: 0.0015
    global_rank: 137
    paper_rank: 137
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Marginal Nodes Matter: Towards Structure Fairness in
      Graphs'
    comparison_source_arxiv: '2310.14527'
    is_best: false
    is_std_outlier: false
  - model: RevGAT
    model_key: revgat
    model_plain: RevGAT
    value: 0.885
    std: 0.002
    paper_value: 0.885
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.885
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.885
    true_std: 0.0005
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.885
    sort_std: 0.0005
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
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.8824
    std: 0.0015
    paper_value: 0.8824
    paper_std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8824
    at_pub_std: 0.015
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8824
    true_std: 0.015
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8824
    sort_std: 0.015
    global_rank: 169
    paper_rank: 169
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
    value: 0.8635
    std: 0.002
    paper_value: 0.8635
    paper_std: 0.002
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.869
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2310.00183'
    at_pub_source_title: On the Equivalence of Graph Convolution and Mixup
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.005499999999999949
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.869
    true_std: 0.0074
    value_gap_source_arxiv: '2310.00183'
    value_gap_source_title: On the Equivalence of Graph Convolution and Mixup
    value_gap_source_is_current_paper: false
    value_gap: 0.005499999999999949
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.0074
    global_rank: 233
    paper_rank: 247
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIANT
    model_key: giant
    model_plain: GIANT
    value: 0.769
    std: 0.002
    paper_value: 0.769
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8275
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2406.11945'
    at_pub_source_title: 'GAugLLM: Improving Graph Contrastive Learning for Text-Attributed
      Graphs with Large Language Models'
    at_pub_source_date_iso: '2024-06-17'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.058499999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8275
    true_std: 0.0028
    value_gap_source_arxiv: '2406.11945'
    value_gap_source_title: 'GAugLLM: Improving Graph Contrastive Learning for Text-Attributed
      Graphs with Large Language Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.058499999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8275
    sort_std: 0.0028
    global_rank: 324
    paper_rank: 773
    rank_delta: 449
    rank_delta_abs: 449
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GAugLLM: Improving Graph Contrastive Learning for Text-Attributed
      Graphs with Large Language Models'
    comparison_source_arxiv: '2406.11945'
    is_best: false
    is_std_outlier: false
  - model: SimTEG
    model_key: simteg
    model_plain: SimTEG
    value: 0.812
    std: 0.0001
    paper_value: 0.812
    paper_std: 0.0001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.812
    true_std: 0.0001
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.812
    sort_std: 0.0001
    global_rank: 380
    paper_rank: 380
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ENGINE
    model_key: engine
    model_plain: ENGINE
    value: 0.7472
    std: 0.0015
    paper_value: 0.7472
    paper_std: 0.0015
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification.
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7472
    true_std: 0.0015
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7472
    sort_std: 0.0015
    global_rank: 832
    paper_rank: 832
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
- &id003
  dataset: ogbn-products
  rows:
  - model: LargeGT-full
    model_key: advsyngnn
    model_plain: LargeGT-full
    value: 0.8931
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.17071'
    title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
      and Self-Corrective Propagation'
    date: Feb 19, 2026
    date_display: Feb 2026
    date_iso: '2026-02-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8931
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LargeGT-full
    model_key: gofa-f
    model_plain: LargeGT-full
    value: 0.8834
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.09709'
    title: 'GOFA: A Generative One-For-All Model for Joint Graph Language Modeling'
    date: Jul 12, 2024
    date_display: Jul 2024
    date_iso: '2024-07-12'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/JiaruiFeng/GOFA
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8834
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LargeGT-full
    model_key: llms
    model_plain: LargeGT-full
    value: 0.882
    std: 0.0005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2412.16441'
    title: 'Towards Graph Foundation Models: Learning Generalities Across Graphs via
      Task-Trees'
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/Zehong-Wang/GIT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.882
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLEM
    model_key: glem
    model_plain: GLEM
    value: 0.7377
    std: 0.0015
    paper_value: 0.7377
    paper_std: 0.0015
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8736
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2308.02565'
    at_pub_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual raph
      Learning'
    at_pub_source_date_iso: '2023-08-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.13590000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8736
    true_std: 0.0007
    value_gap_source_arxiv: '2308.02565'
    value_gap_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual raph
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.13590000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8736
    sort_std: 0.0007
    global_rank: 6
    paper_rank: 302
    rank_delta: 296
    rank_delta_abs: 296
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual
      raph Learning'
    comparison_source_arxiv: '2308.02565'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7052
    std: 0.0012
    paper_value: 0.7052
    paper_std: 0.0012
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8868
    at_pub_std: null
    at_pub_source_arxiv: '2505.19762'
    at_pub_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    at_pub_source_date_iso: '2025-05-26'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.18159999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8691
    true_std: 0.0005
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.16389999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8691
    sort_std: 0.0005
    global_rank: 12
    paper_rank: 332
    rank_delta: 320
    rank_delta_abs: 320
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    comparison_source_arxiv: '2505.19762'
    is_best: false
    is_std_outlier: false
  - model: SimTEG
    model_key: simteg
    model_plain: SimTEG
    value: 0.7451
    std: 0.002
    paper_value: 0.7451
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.854
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2308.02565'
    at_pub_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual raph
      Learning'
    at_pub_source_date_iso: '2023-08-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.1089
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.854
    true_std: 0.0028
    value_gap_source_arxiv: '2308.02565'
    value_gap_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual raph
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.1089
    has_value_note: false
    value_note: ''
    sort_value: 0.854
    sort_std: 0.0028
    global_rank: 27
    paper_rank: 283
    rank_delta: 256
    rank_delta_abs: 256
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual
      raph Learning'
    comparison_source_arxiv: '2308.02565'
    is_best: false
    is_std_outlier: false
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.6815
    std: 0.0012
    paper_value: 0.6815
    paper_std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7934
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2405.19779'
    at_pub_source_title: Automatic Graph Topology-Aware Transformer
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-02-19'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.1119
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8418
    true_std: 0.0015
    value_gap_source_arxiv: '2602.17071'
    value_gap_source_title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial
      Synthesis and Self-Corrective Propagation'
    value_gap_source_is_current_paper: false
    value_gap: 0.1603
    has_value_note: false
    value_note: ''
    sort_value: 0.8418
    sort_std: 0.0015
    global_rank: 44
    paper_rank: 344
    rank_delta: 300
    rank_delta_abs: 300
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Automatic Graph Topology-Aware Transformer
    comparison_source_arxiv: '2405.19779'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.6913
    std: 0.002
    paper_value: 0.6913
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8933
    at_pub_std: null
    at_pub_source_arxiv: '2505.19762'
    at_pub_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    at_pub_source_date_iso: '2025-05-26'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.20199999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8233
    true_std: 0.0037
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: false
    value_gap: 0.132
    has_value_note: false
    value_note: ''
    sort_value: 0.8233
    sort_std: 0.0037
    global_rank: 84
    paper_rank: 342
    rank_delta: 258
    rank_delta_abs: 258
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    comparison_source_arxiv: '2505.19762'
    is_best: false
    is_std_outlier: false
  - model: GIANT
    model_key: giant
    model_plain: GIANT
    value: 0.7406
    std: 0.0012
    paper_value: 0.7406
    paper_std: 0.0012
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8049
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2304.10668'
    at_pub_source_title: 'Train Your Own GNN Teacher: Graph-Aware Distillation on
      Textual Graphs'
    at_pub_source_date_iso: '2023-04-20'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06429999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8049
    true_std: 0.0028
    value_gap_source_arxiv: '2304.10668'
    value_gap_source_title: 'Train Your Own GNN Teacher: Graph-Aware Distillation
      on Textual Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.06429999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.8049
    sort_std: 0.0028
    global_rank: 132
    paper_rank: 290
    rank_delta: 158
    rank_delta_abs: 158
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Train Your Own GNN Teacher: Graph-Aware Distillation
      on Textual Graphs'
    comparison_source_arxiv: '2304.10668'
    is_best: false
    is_std_outlier: false
  - model: ENGINE
    model_key: engine
    model_plain: ENGINE
    value: 0.8005
    std: 0.0015
    paper_value: 0.8005
    paper_std: 0.0015
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8005
    at_pub_std: 0.0045
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8005
    true_std: 0.0015
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8005
    sort_std: 0.0015
    global_rank: 143
    paper_rank: 143
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TAPE
    model_key: tape
    model_plain: TAPE
    value: 0.7996
    std: 0.002
    paper_value: 0.7996
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8234
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2502.13555'
    at_pub_source_title: Democratizing Large Language Model-Based Graph Data Augmentation
      via Latent Knowledge Graphs
    at_pub_source_date_iso: '2025-02-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.023800000000000043
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7996
    true_std: 0.002
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7996
    sort_std: 0.002
    global_rank: 146
    paper_rank: 146
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Democratizing Large Language Model-Based Graph Data Augmentation
      via Latent Knowledge Graphs
    comparison_source_arxiv: '2502.13555'
    is_best: false
    is_std_outlier: false
  - model: GAGA
    model_key: gaga
    model_plain: GAGA
    value: 0.7887
    std: 0.0018
    paper_value: 0.7887
    paper_std: 0.0018
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7887
    true_std: 0.0018
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7887
    sort_std: 0.0018
    global_rank: 200
    paper_rank: 200
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RevGAT
    model_key: revgat
    model_plain: RevGAT
    value: 0.6964
    std: 0.0015
    paper_value: 0.6964
    paper_std: 0.0015
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8859
    at_pub_std: null
    at_pub_source_arxiv: '2505.19762'
    at_pub_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    at_pub_source_date_iso: '2025-05-26'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.1895
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6964
    true_std: 0.0015
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6964
    sort_std: 0.0015
    global_rank: 340
    paper_rank: 340
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    comparison_source_arxiv: '2505.19762'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5385
    std: 0.0018
    paper_value: 0.5385
    paper_std: 0.0018
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8418
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2112.04319'
    at_pub_source_title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    at_pub_source_date_iso: '2021-12-08'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-11-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.3033
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6605
    true_std: 0.002
    value_gap_source_arxiv: '2211.16199'
    value_gap_source_title: Latent Graph Inference using Product Manifolds
    value_gap_source_is_current_paper: false
    value_gap: 0.122
    has_value_note: false
    value_note: ''
    sort_value: 0.6605
    sort_std: 0.002
    global_rank: 353
    paper_rank: 380
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SCR: Training Graph Neural Networks with Consistency
      Regularization'
    comparison_source_arxiv: '2112.04319'
    is_best: false
    is_std_outlier: false
  - model: InstructGLM
    model_key: instructglm
    model_plain: InstructGLM
    value: 0.6532
    std: 0.0002
    paper_value: 0.6532
    paper_std: 0.0002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ogbn-products node classification
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6532
    true_std: 0.0002
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6532
    sort_std: 0.0002
    global_rank: 357
    paper_rank: 357
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
- benchmark: Classic
  datasets:
  - *id001
  - *id002
- benchmark: OGB
  datasets:
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: PubMed
      dataset_slug: pubmed
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
single_proposed_model: GAGA
main_figure: /figures/2506.07168/main_figure.jpegoptim.jpg
---

