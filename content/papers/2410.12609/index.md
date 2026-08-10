---
title: 'Towards Graph Foundation Models: Training on Knowledge Graphs Enables Transferability
  to General Graphs'
arxiv_id: '2410.12609'
source_url: ''
authors:
- name: Kai Wang
  orcid: null
  s2_author_id: '2326276530'
  s2_url: null
- name: Siqiang Luo
  orcid: null
  s2_author_id: '2284759164'
  s2_url: null
- name: Caihua Shan
  orcid: null
  s2_author_id: '145663545'
  s2_url: null
- name: Yifei Shen
  orcid: null
  s2_author_id: '2152966656'
  s2_url: null
published_date: Oct 16, 2024
published_date_iso: '2024-10-16'
published_venue: NeurIPS 2024
published_conference: NeurIPS 2024
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Inspired by the success of large language models, there is a trend toward
  developing graph foundation models to conduct diverse downstream tasks in various
  domains. However, current models often require extra fine-tuning to apply their
  learned structural and semantic representations to new graphs, which limits their
  versatility. Recent breakthroughs in zero-shot inductive reasoning on knowledge
  graphs (KGs), offer us a new perspective on extending KG reasoning to general graph
  applications. In this paper, we introduce SCR, a unified graph reasoning framework
  designed to train on knowledge graphs and effectively generalize across a wide range
  of graph tasks and domains. We begin by designing the task-specific KG structures
  to establish a unified topology for different task formats. Then we propose semantic-conditioned
  message passing, a novel mechanism addressing the inherent semantic isolation in
  traditional KG reasoning, by jointly modeling structural and semantic invariance
  patterns in graph representations. To demonstrate the effectiveness, we evaluate
  the inductive reasoning capability of SCR using 38 diverse graph datasets, covering
  node-level, link-level, and graph-level tasks across multiple domains. Our results
  show substantial performance gains over existing foundation models and supervised
  baselines, highlighting the efficacy and adaptability of our approach.
codebase_url: https://github.com/DeepGraphLearning/ULTRA
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Knowledge Graphs
benchmark_coverage:
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 1
  total: 3
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id001
  dataset: WN18RR
  rows:
  - model: PNA, Msg_r^2, f(t)=t
    model_key: pna, msg_r^2, f(t)=t
    model_plain: PNA, Msg_r^2, f(t)=t
    value: 0.947
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_display: Feb 2023
    date_iso: '2023-02-04'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.947
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PNA, Msg_r^3, f(t)=0
    model_key: pna, msg_r^3, f(t)=0
    model_plain: PNA, Msg_r^3, f(t)=0
    value: 0.947
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_display: Feb 2023
    date_iso: '2023-02-04'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.947
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PNA, Msg_r^2, f(t)=0
    model_key: pna, msg_r^2, f(t)=0
    model_plain: PNA, Msg_r^2, f(t)=0
    value: 0.946
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_display: Feb 2023
    date_iso: '2023-02-04'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.946
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8298
    std: 0.0022
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
    global_rank: 25
    sort_value: 0.8298
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Supervised SOTA
    model_key: supervised sota
    model_plain: Supervised SOTA
    value: 0.64
    std: null
    paper_value: 0.64
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 16, 2024
    date_display: Oct 2024
    date_iso: '2024-10-16'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.551
    at_pub_std: null
    at_pub_source_arxiv: '2310.04562'
    at_pub_source_title: Towards Foundation Models for Knowledge Graph Reasoning
    at_pub_source_date_iso: '2023-10-06'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-10-16'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.08899999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.64
    true_std: null
    value_gap_source_arxiv: '2410.12609'
    value_gap_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.64
    sort_std: null
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Towards Foundation Models for Knowledge Graph Reasoning
    comparison_source_arxiv: '2310.04562'
    is_best: false
    is_std_outlier: false
  - model: SCR-MPNet
    model_key: scr-mpnet
    model_plain: SCR-MPNet
    value: 0.578
    std: null
    paper_value: 0.578
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
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
    true_value: 0.578
    true_std: null
    value_gap_source_arxiv: '2410.12609'
    value_gap_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.578
    sort_std: null
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
  - model: SCR(3g)
    model_key: scr(3g)
    model_plain: SCR(3g)
    value: 0.576
    std: null
    paper_value: 0.576
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
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
    true_value: 0.576
    true_std: null
    value_gap_source_arxiv: '2410.12609'
    value_gap_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.576
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
  - model: SCR-MiniLM
    model_key: scr-minilm
    model_plain: SCR-MiniLM
    value: 0.576
    std: null
    paper_value: 0.576
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
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
    true_value: 0.576
    true_std: null
    value_gap_source_arxiv: '2410.12609'
    value_gap_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.576
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
  - model: SCR-DistilBert
    model_key: scr-distilbert
    model_plain: SCR-DistilBert
    value: 0.576
    std: null
    paper_value: 0.576
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
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
    true_value: 0.576
    true_std: null
    value_gap_source_arxiv: '2410.12609'
    value_gap_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.576
    sort_std: null
    global_rank: 46
    paper_rank: 46
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SCR-Ontology
    model_key: scr-ontology
    model_plain: SCR-Ontology
    value: 0.57
    std: null
    paper_value: 0.57
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
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
    true_value: 0.57
    true_std: null
    value_gap_source_arxiv: '2410.12609'
    value_gap_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.57
    sort_std: null
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SCR-One
    model_key: scr-one
    model_plain: SCR-One
    value: 0.569
    std: null
    paper_value: 0.569
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
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
    true_value: 0.569
    true_std: null
    value_gap_source_arxiv: '2410.12609'
    value_gap_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.569
    sort_std: null
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
  - model: ULTRA(4g)
    model_key: ultra(4g)
    model_plain: ULTRA(4g)
    value: 0.567
    std: null
    paper_value: 0.567
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
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
    true_value: 0.567
    true_std: null
    value_gap_source_arxiv: '2410.12609'
    value_gap_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.567
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
  - model: ProLINK(3g)
    model_key: prolink(3g)
    model_plain: ProLINK(3g)
    value: 0.553
    std: null
    paper_value: 0.553
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
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
    true_value: 0.553
    true_std: null
    value_gap_source_arxiv: '2410.12609'
    value_gap_source_title: 'Towards Graph Foundation Models: Training on Knowledge
      Graphs Enables Transferability to General Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.553
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
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: WN18RR
      dataset_slug: wn18rr
main_figure: /figures/2410.12609/main_figure.jpegoptim.jpg
---

