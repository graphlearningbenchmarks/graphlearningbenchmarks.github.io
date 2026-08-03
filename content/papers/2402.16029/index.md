---
title: 'GraphWiz: An Instruction-Following Language Model for Graph Computational
  Problems'
arxiv_id: '2402.16029'
source_url: ''
authors:
- name: Nuo Chen
  orcid: null
  s2_author_id: '2263638230'
  s2_url: null
- name: Yuhan Li
  orcid: null
  s2_author_id: '2267495002'
  s2_url: null
- name: Jianheng Tang
  orcid: null
  s2_author_id: '2287915481'
  s2_url: null
- name: Jia Li
  orcid: null
  s2_author_id: '2273828439'
  s2_url: null
published_date: Feb 25, 2024
published_date_iso: '2024-02-25'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Large language models (LLMs) have achieved impressive success across various
  domains, but their capability in understanding and resolving complex graph problems
  is less explored. To bridge this gap, we introduce GraphInstruct, a novel instruction-tuning
  dataset aimed at enabling language models to tackle a broad spectrum of graph problems
  through explicit reasoning paths. Utilizing GraphInstruct, we build GraphWiz, an
  open-source language model capable of solving various graph computational problems
  while generating clear reasoning processes. To further enhance the model's performance
  and reliability, we integrate the Direct Preference Optimization (DPO) framework
  within the graph problem-solving context. The improved model, GraphWiz-DPO, achieves
  an average accuracy of 65\
codebase_url: https://github.com/nuochenpku/Graph-Reasoning-LLM
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraphWiz (LLaMA 2-13B)
- GraphWiz-DPO (LLaMA 2-7B)
- GraphWiz
mrr: 0.3333
adjusted_mrr: 0.1111
mrr_dataset_count: 1
benchmark_categories:
- GraphBench
benchmark_coverage:
- benchmark: GraphBench
  benchmark_slug: graphbench
  evaluated: 2
  total: 5
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: BA graph
  rows:
  - model: GraphWiz
    model_key: f4-mpnn
    model_plain: GraphWiz
    value: 0.9793
    std: 0.0068
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    venue: arXiv.org
    codebase_url: https://github.com/RPaolino/GenVsExp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9793
    sort_std: 0.0068
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphWiz
    model_key: f7-mpnn
    model_plain: GraphWiz
    value: 0.966
    std: 0.0065
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    venue: arXiv.org
    codebase_url: https://github.com/RPaolino/GenVsExp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.0065
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphWiz
    model_key: f3-mpnn
    model_plain: GraphWiz
    value: 0.8657
    std: 0.0085
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    venue: arXiv.org
    codebase_url: https://github.com/RPaolino/GenVsExp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8657
    sort_std: 0.0085
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphWiz
    model_key: graphwiz
    model_plain: GraphWiz
    value: 0.6812
    std: null
    paper_value: 0.6812
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Additional Experiments text
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average accuracy reported for BA graphs across six tasks (Cycle,
      Connectivity, Bipartite, Hamilton, Shortest, and Flow) with 200 examples each.
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6812
    true_std: null
    value_gap_source_arxiv: '2402.16029'
    value_gap_source_title: 'GraphWiz: An Instruction-Following Language Model for
      Graph Computational Problems'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6812
    sort_std: null
    global_rank: 8
    paper_rank: 8
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
- &id001
  dataset: ER graph
  rows:
  - model: GraphWiz-DPO (LLaMA 2-7B)
    model_key: f_4-mpnn
    model_plain: GraphWiz-DPO (LLaMA 2-7B)
    value: 0.9793
    std: 0.0068
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    venue: arXiv.org
    codebase_url: https://github.com/RPaolino/GenVsExp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9793
    sort_std: 0.0068
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphWiz-DPO (LLaMA 2-7B)
    model_key: f_7-mpnn
    model_plain: GraphWiz-DPO (LLaMA 2-7B)
    value: 0.966
    std: 0.0065
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    venue: arXiv.org
    codebase_url: https://github.com/RPaolino/GenVsExp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.0065
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphWiz (LLaMA 2-13B)
    model_key: graphwiz (llama 2-13b)
    model_plain: GraphWiz (LLaMA 2-13B)
    value: 0.9475
    std: null
    paper_value: 0.9475
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluated on GraphInstruct test set which uses ER graphs.
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9475
    true_std: null
    value_gap_source_arxiv: '2402.16029'
    value_gap_source_title: 'GraphWiz: An Instruction-Following Language Model for
      Graph Computational Problems'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9475
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
  - model: GraphWiz-DPO (LLaMA 2-7B)
    model_key: graphwiz-dpo (llama 2-7b)
    model_plain: GraphWiz-DPO (LLaMA 2-7B)
    value: 0.89
    std: null
    paper_value: 0.89
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluated on GraphInstruct test set which uses ER graphs.
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.89
    true_std: null
    value_gap_source_arxiv: '2402.16029'
    value_gap_source_title: 'GraphWiz: An Instruction-Following Language Model for
      Graph Computational Problems'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.89
    sort_std: null
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.875
    std: null
    paper_value: 0.875
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluated on GraphInstruct test set which uses ER graphs.
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.875
    true_std: null
    value_gap_source_arxiv: '2402.16029'
    value_gap_source_title: 'GraphWiz: An Instruction-Following Language Model for
      Graph Computational Problems'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.875
    sort_std: null
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.875
    std: null
    paper_value: 0.875
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluated on GraphInstruct test set which uses ER graphs.
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.875
    true_std: null
    value_gap_source_arxiv: '2402.16029'
    value_gap_source_title: 'GraphWiz: An Instruction-Following Language Model for
      Graph Computational Problems'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.875
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.84
    std: null
    paper_value: 0.84
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluated on GraphInstruct test set which uses ER graphs.
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.85
    at_pub_std: null
    at_pub_source_arxiv: '1710.10321'
    at_pub_source_title: Learning Structural Node Embeddings via Diffusion Wavelets
    at_pub_source_date_iso: '2017-10-27'
    at_pub_source_date_label: KDD 2017
    value_gap_source_date_iso: '2024-02-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.010000000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.84
    true_std: null
    value_gap_source_arxiv: '2402.16029'
    value_gap_source_title: 'GraphWiz: An Instruction-Following Language Model for
      Graph Computational Problems'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.84
    sort_std: null
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning Structural Node Embeddings via Diffusion Wavelets
    comparison_source_arxiv: '1710.10321'
    is_best: false
    is_std_outlier: false
  - model: GPT-4 (2-shot)
    model_key: gpt-4 (2-shot)
    model_plain: GPT-4 (2-shot)
    value: 0.525
    std: null
    paper_value: 0.525
    paper_std: null
    metric: Accuracy
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluated on GraphInstruct test set which uses ER graphs.
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.525
    true_std: null
    value_gap_source_arxiv: '2402.16029'
    value_gap_source_title: 'GraphWiz: An Instruction-Following Language Model for
      Graph Computational Problems'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.525
    sort_std: null
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPT-3.5 (2-shot)
    model_key: gpt-3.5 (2-shot)
    model_plain: GPT-3.5 (2-shot)
    value: 0.5125
    std: null
    paper_value: 0.5125
    paper_std: null
    metric: Accuracy
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluated on GraphInstruct test set which uses ER graphs.
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5125
    true_std: null
    value_gap_source_arxiv: '2402.16029'
    value_gap_source_title: 'GraphWiz: An Instruction-Following Language Model for
      Graph Computational Problems'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5125
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: GraphBench
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: GraphBench
    benchmark_slug: graphbench
    datasets:
    - dataset: ER graph
      dataset_slug: er-graph
    - dataset: BA graph
      dataset_slug: ba-graph
---

