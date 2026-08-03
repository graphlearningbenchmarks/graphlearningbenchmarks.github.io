---
title: A Prompt-Based Knowledge Graph Foundation Model for Universal In-Context Reasoning
arxiv_id: '2410.12288'
source_url: ''
authors:
- name: Yuanning Cui
  orcid: null
  s2_author_id: '1410917541'
  s2_url: null
- name: Zequn Sun
  orcid: null
  s2_author_id: '2109745316'
  s2_url: null
- name: Wei Hu
  orcid: null
  s2_author_id: '2311649985'
  s2_url: null
published_date: Oct 16, 2024
published_date_iso: '2024-10-16'
published_venue: NeurIPS 2024
published_conference: NeurIPS 2024
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Extensive knowledge graphs (KGs) have been constructed to facilitate knowledge-driven
  tasks across various scenarios. However, existing work usually develops separate
  reasoning models for different KGs, lacking the ability to generalize and transfer
  knowledge across diverse KGs and reasoning settings. In this paper, we propose a
  prompt-based KG foundation model via in-context learning, namely KG-ICL, to achieve
  a universal reasoning ability. Specifically, we introduce a prompt graph centered
  with a query-related example fact as context to understand the query relation. To
  encode prompt graphs with the generalization ability to unseen entities and relations
  in queries, we first propose a unified tokenizer that maps entities and relations
  in prompt graphs to predefined tokens. Then, we propose two message passing neural
  networks to perform prompt encoding and KG reasoning, respectively. We conduct evaluation
  on 43 different KGs in both transductive and inductive settings. Results indicate
  that the proposed KG-ICL outperforms baselines on most datasets, showcasing its
  outstanding generalization and universal reasoning capabilities. The source code
  is accessible on GitHub:.
codebase_url: https://github.com/nju-websoft/KG-ICL
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- KG-ICL pre-train
- KG-ICL finetune
mrr: 0.0159
adjusted_mrr: 0.0053
mrr_dataset_count: 1
benchmark_categories:
- Knowledge Graphs
benchmark_coverage:
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 2
  total: 3
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id002
  dataset: FB15k-237
  is_multi_metric: true
  rows:
  - model: CompGCN
    model_key: llms
    model_plain: CompGCN
    metric_values:
    - 0.815
    - null
    metric_stds:
    - 0.023
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    published_venue: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.815
    sort_std: 0.023
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
  - model: CompGCN
    model_key: gcope
    model_plain: CompGCN
    metric_values:
    - 0.793
    - null
    metric_stds:
    - 0.022
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    published_venue: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.793
    sort_std: 0.022
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
  - model: CompGCN
    model_key: gft
    model_plain: CompGCN
    metric_values:
    - 0.791
    - null
    metric_stds:
    - 0.016
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    published_venue: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: true
    sort_value: 0.791
    sort_std: 0.016
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
  - model: KG-ICL pre-train
    model_key: kg-icl pre-train
    model_plain: KG-ICL pre-train
    metric_values:
    - 0.329
    - 0.433
    metric_stds:
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.329
    sort_std: null
    true_value: 0.329
    true_std: null
    paper_value: 0.329
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.12288'
    value_gap_source_title: A Prompt-Based Knowledge Graph Foundation Model for Universal
      In-Context Reasoning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
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
    published_venue: NeurIPS 2024
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 57
  - model: ULTRA finetune
    model_key: ultra finetune
    model_plain: ULTRA finetune
    metric_values:
    - 0.325
    - 0.411
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.325
    sort_std: null
    true_value: 0.325
    true_std: null
    paper_value: 0.325
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.12288'
    value_gap_source_title: A Prompt-Based Knowledge Graph Foundation Model for Universal
      In-Context Reasoning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
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
    published_venue: NeurIPS 2024
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 60
  - model: KG-ICL finetune
    model_key: kg-icl finetune
    model_plain: KG-ICL finetune
    metric_values:
    - 0.324
    - 0.416
    metric_stds:
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.324
    sort_std: null
    true_value: 0.324
    true_std: null
    paper_value: 0.324
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.12288'
    value_gap_source_title: A Prompt-Based Knowledge Graph Foundation Model for Universal
      In-Context Reasoning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
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
    published_venue: NeurIPS 2024
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 63
  - model: ULTRA pre-train
    model_key: ultra pre-train
    model_plain: ULTRA pre-train
    metric_values:
    - 0.324
    - 0.398
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.324
    sort_std: null
    true_value: 0.324
    true_std: null
    paper_value: 0.324
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.12288'
    value_gap_source_title: A Prompt-Based Knowledge Graph Foundation Model for Universal
      In-Context Reasoning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
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
    published_venue: NeurIPS 2024
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 62
  - model: Supervised SOTA
    model_key: supervised sota
    model_plain: Supervised SOTA
    metric_values:
    - 0.293
    - 0.337
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.293
    sort_std: null
    true_value: 0.293
    true_std: null
    paper_value: 0.293
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.12288'
    value_gap_source_title: A Prompt-Based Knowledge Graph Foundation Model for Universal
      In-Context Reasoning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
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
    published_venue: NeurIPS 2024
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 67
  metrics:
  - MRR
  - H@10
  primary_metric: MRR
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - H@10
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: WN18RR
  rows:
  - model: CompGCN
    model_key: gft
    model_plain: CompGCN
    value: 0.9191
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06070'
    title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    date: Nov 9, 2024
    date_display: Nov 2024
    date_iso: '2024-11-09'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/Zehong-Wang/GFT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9191
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CompGCN
    model_key: unigraph2
    model_plain: CompGCN
    value: 0.8786
    std: 0.0006
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2502.00806'
    title: 'UniGraph2: Learning a Unified Embedding Space to Bind Multimodal Graphs'
    date: Feb 2, 2025
    date_display: Feb 2025
    date_iso: '2025-02-02'
    venue: The Web Conference
    codebase_url: https://github.com/yf-he/UniGraph2
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8786
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CompGCN
    model_key: gat
    model_plain: CompGCN
    value: 0.8552
    std: 0.0012
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: Accepted by NeurIPS 2025
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8552
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Supervised SOTA
    model_key: supervised sota
    model_plain: Supervised SOTA
    value: 0.551
    std: null
    paper_value: 0.551
    paper_std: null
    metric: MRR
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard transductive link prediction on WN18RR
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.64
    at_pub_std: null
    at_pub_source_arxiv: '2410.12609'
    at_pub_source_title: 'Towards Graph Foundation Models: Training on Knowledge Graphs
      Enables Transferability to General Graphs'
    at_pub_source_date_iso: '2024-10-16'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2023-10-06'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.08899999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.551
    true_std: null
    value_gap_source_arxiv: '2310.04562'
    value_gap_source_title: Towards Foundation Models for Knowledge Graph Reasoning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.551
    sort_std: null
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    comparison_source_arxiv: '2410.12609'
    is_best: false
    is_std_outlier: false
  - model: KG-ICL finetune
    model_key: kg-icl finetune
    model_plain: KG-ICL finetune
    value: 0.536
    std: null
    paper_value: 0.536
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard transductive link prediction on WN18RR
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.536
    true_std: null
    value_gap_source_arxiv: '2410.12288'
    value_gap_source_title: A Prompt-Based Knowledge Graph Foundation Model for Universal
      In-Context Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.536
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
  - model: ULTRA pre-train
    model_key: ultra pre-train
    model_plain: ULTRA pre-train
    value: 0.48
    std: null
    paper_value: 0.48
    paper_std: null
    metric: MRR
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
    source_ref: ULTRA
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard transductive link prediction on WN18RR
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.48
    true_std: null
    value_gap_source_arxiv: '2410.12288'
    value_gap_source_title: A Prompt-Based Knowledge Graph Foundation Model for Universal
      In-Context Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.48
    sort_std: null
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ULTRA finetune
    model_key: ultra finetune
    model_plain: ULTRA finetune
    value: 0.48
    std: null
    paper_value: 0.48
    paper_std: null
    metric: MRR
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
    source_ref: ULTRA
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard transductive link prediction on WN18RR
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.48
    true_std: null
    value_gap_source_arxiv: '2410.12288'
    value_gap_source_title: A Prompt-Based Knowledge Graph Foundation Model for Universal
      In-Context Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.48
    sort_std: null
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KG-ICL pre-train
    model_key: kg-icl pre-train
    model_plain: KG-ICL pre-train
    value: 0.455
    std: null
    paper_value: 0.455
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard transductive link prediction on WN18RR
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.455
    true_std: null
    value_gap_source_arxiv: '2410.12288'
    value_gap_source_title: A Prompt-Based Knowledge Graph Foundation Model for Universal
      In-Context Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.455
    sort_std: null
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
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Knowledge Graphs
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: WN18RR
      dataset_slug: wn18rr
    - dataset: FB15k-237
      dataset_slug: fb15k-237
---

