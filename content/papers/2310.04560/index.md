---
title: 'Talk like a Graph: Encoding Graphs for Large Language Models'
arxiv_id: '2310.04560'
source_url: ''
authors:
- name: Bahare Fatemi
  orcid: null
  s2_author_id: '3422551'
  s2_url: null
- name: Jonathan J. Halcrow
  orcid: null
  s2_author_id: '101461191'
  s2_url: null
- name: Bryan Perozzi
  orcid: null
  s2_author_id: '2271808'
  s2_url: null
published_date: Oct 6, 2023
published_date_iso: '2023-10-06'
published_venue: ICLR 2023
published_conference: ICLR 2023
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'Graphs are a powerful tool for representing and analyzing complex relationships
  in real-world applications such as social networks, recommender systems, and computational
  finance. Reasoning on graphs is essential for drawing inferences about the relationships
  between entities in a complex system, and to identify hidden patterns and trends.
  Despite the remarkable progress in automated reasoning with natural text, reasoning
  on graphs with large language models (LLMs) remains an understudied problem. In
  this work, we perform the first comprehensive study of encoding graph-structured
  data as text for consumption by LLMs. We show that LLM performance on graph reasoning
  tasks varies on three fundamental levels: (1) the graph encoding method, (2) the
  nature of the graph task itself, and (3) interestingly, the very structure of the
  graph considered. These novel results provide valuable insight on strategies for
  encoding graphs as text. Using these insights we illustrate how the correct choice
  of encoders can boost performance on graph reasoning tasks inside LLMs by 4.8\'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- GraphBench
benchmark_coverage:
- benchmark: GraphBench
  benchmark_slug: graphbench
  evaluated: 2
  total: 8
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: BA graph
  rows:
  - model: F4-MPNN
    model_key: f4-mpnn
    model_plain: F4-MPNN
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
  - model: F7-MPNN
    model_key: f7-mpnn
    model_plain: F7-MPNN
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
  - model: Diffusion Wavelets
    model_key: diffusion wavelets
    model_plain: Diffusion Wavelets
    value: 0.94
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_display: Oct 2017
    date_iso: '2017-10-27'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.94
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.85
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
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_display: Oct 2017
    date_iso: '2017-10-27'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 7
    sort_value: 0.85
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Zero-shot
    model_key: zero-shot
    model_plain: Zero-shot
    value: 0.502
    std: null
    paper_value: 0.502
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Zero-shot prompting on BA graph generator
    date: Oct 6, 2023
    date_display: Oct 2023
    date_iso: '2023-10-06'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-06'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.502
    true_std: null
    value_gap_source_arxiv: '2310.04560'
    value_gap_source_title: 'Talk like a Graph: Encoding Graphs for Large Language
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.502
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
  - model: CoT
    model_key: cot
    model_plain: CoT
    value: 0.4
    std: null
    paper_value: 0.4
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: CoT prompting on BA graph generator
    date: Oct 6, 2023
    date_display: Oct 2023
    date_iso: '2023-10-06'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-06'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4
    true_std: null
    value_gap_source_arxiv: '2310.04560'
    value_gap_source_title: 'Talk like a Graph: Encoding Graphs for Large Language
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4
    sort_std: null
    global_rank: 15
    paper_rank: 15
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
- &id002
  dataset: ER graph
  rows:
  - model: F_4-MPNN
    model_key: f_4-mpnn
    model_plain: F_4-MPNN
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
  - model: F_7-MPNN
    model_key: f_7-mpnn
    model_plain: F_7-MPNN
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
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2402.16029'
    title: 'GraphWiz: An Instruction-Following Language Model for Graph Computational
      Problems'
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    venue: null
    codebase_url: https://github.com/nuochenpku/Graph-Reasoning-LLM
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9475
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.88
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
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_display: Oct 2017
    date_iso: '2017-10-27'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 6
    sort_value: 0.88
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Zero-shot
    model_key: zero-shot
    model_plain: Zero-shot
    value: 0.451
    std: null
    paper_value: 0.451
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Zero-shot prompting on ER graphs using PaLM 62B
    date: Oct 6, 2023
    date_display: Oct 2023
    date_iso: '2023-10-06'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-06'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.451
    true_std: null
    value_gap_source_arxiv: '2310.04560'
    value_gap_source_title: 'Talk like a Graph: Encoding Graphs for Large Language
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.451
    sort_std: null
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CoT
    model_key: cot
    model_plain: CoT
    value: 0.412
    std: null
    paper_value: 0.412
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: CoT prompting on ER graphs using PaLM 62B
    date: Oct 6, 2023
    date_display: Oct 2023
    date_iso: '2023-10-06'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-06'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.412
    true_std: null
    value_gap_source_arxiv: '2310.04560'
    value_gap_source_title: 'Talk like a Graph: Encoding Graphs for Large Language
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.412
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
    - dataset: BA graph
      dataset_slug: ba-graph
    - dataset: ER graph
      dataset_slug: er-graph
main_figure: /figures/2310.04560/main_figure.jpegoptim.jpg
---

