---
title: Towards Foundation Models for Knowledge Graph Reasoning
arxiv_id: '2310.04562'
source_url: ''
authors:
- name: Mikhail Galkin
  orcid: null
  s2_author_id: '2066369448'
  s2_url: null
- name: Xinyu Yuan
  orcid: null
  s2_author_id: '2258299935'
  s2_url: null
- name: Hesham Mostafa
  orcid: null
  s2_author_id: '2256992354'
  s2_url: null
- name: Jian Tang
  orcid: null
  s2_author_id: '2255480226'
  s2_url: null
- name: Zhaocheng Zhu
  orcid: null
  s2_author_id: '9031926'
  s2_url: null
published_date: Oct 6, 2023
published_date_iso: '2023-10-06'
published_venue: ICLR 2023
published_conference: ICLR 2023
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Foundation models in language and vision have the ability to run inference
  on any textual and visual inputs thanks to the transferable representations such
  as a vocabulary of tokens in language. Knowledge graphs (KGs) have different entity
  and relation vocabularies that generally do not overlap. The key challenge of designing
  foundation models on KGs is to learn such transferable representations that enable
  inference on any graph with arbitrary entity and relation vocabularies. In this
  work, we make a step towards such foundation models and present Ultra, an approach
  for learning universal and transferable graph representations. Ultra builds relational
  representations as a function conditioned on their interactions. Such a conditioning
  strategy allows a pre-trained Ultra model to inductively generalize to any unseen
  KG with any relation vocabulary and to be fine-tuned on any graph. Conducting link
  prediction experiments on 57 different KGs, we find that the zero-shot inductive
  inference performance of a single pre-trained Ultra model on unseen graphs of various
  sizes is often on par or better than strong baselines trained on specific graphs.
  Fine-tuning further boosts the performance. The code is available:.
codebase_url: https://github.com/DeepGraphLearning/ULTRA
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Ultra fine-tuned
mrr: 0.0233
adjusted_mrr: 0.0078
mrr_dataset_count: 1
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
    protocol_note: Fine-tuning regime on pre-training dataset WN18RR
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
    true_value: 0.551
    true_std: null
    value_gap_source_arxiv: '2310.04562'
    value_gap_source_title: Towards Foundation Models for Knowledge Graph Reasoning
    value_gap_source_is_current_paper: true
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
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Ultra fine-tuned
    model_key: ultra fine-tuned
    model_plain: Ultra fine-tuned
    value: 0.48
    std: null
    paper_value: 0.48
    paper_std: null
    metric: MRR
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Fine-tuning regime on pre-training dataset WN18RR
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
    true_value: 0.48
    true_std: null
    value_gap_source_arxiv: '2310.04562'
    value_gap_source_title: Towards Foundation Models for Knowledge Graph Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.48
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
single_proposed_model: Ultra fine-tuned
main_figure: /figures/2310.04562/main_figure.jpegoptim.jpg
---

