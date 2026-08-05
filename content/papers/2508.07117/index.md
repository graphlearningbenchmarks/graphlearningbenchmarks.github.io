---
title: 'From Nodes to Narratives: Explaining Graph Neural Networks with LLMs and Graph
  Context'
arxiv_id: '2508.07117'
source_url: ''
authors:
- name: Peyman Baghershahi
  orcid: null
  s2_author_id: '2146375278'
  s2_url: null
- name: Gregoire Fournier
  orcid: null
  s2_author_id: '2362724871'
  s2_url: null
- name: Pranav Nyati
  orcid: null
  s2_author_id: '2370928970'
  s2_url: null
- name: Sourav Medya
  orcid: null
  s2_author_id: '3390598'
  s2_url: null
published_date: Aug 9, 2025
published_date_iso: '2025-08-09'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) have emerged as powerful tools for learning
  over structured data, including text-attributed graphs (TAGs), which are common
  in domains such as citation networks, social platforms, and knowledge graphs. GNNs
  are not inherently interpretable and thus, many explanation methods have been proposed.
  However, existing explanation methods often struggle to generate interpretable,
  fine-grained rationales, especially when node attributes include rich natural language.
  In this work, we introduce Gspell, a lightweight, post-hoc framework that uses large
  language models (LLMs) to generate faithful and interpretable explanations for GNN
  predictions. Gspell projects GNN node embeddings into the LLM embedding space and
  constructs hybrid prompts that interleave soft prompts with textual inputs from
  the graph structure. This enables the LLM to reason about GNN internal representations
  and to produce natural-language explanations, along with concise explanation subgraphs.
  Our experiments across real-world TAG datasets demonstrate that Gspell achieves
  a favorable trade-off between fidelity and sparsity, while improving human-centric
  metrics such as insightfulness. Gspell sets a new direction for LLM-based explainability
  in graph learning by aligning GNN internals with human reasoning.
codebase_url: https://github.com/pbaghershahi/GSPELL.git
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Gspell+
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: Amazon2M
  rows:
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    value: 0.945
    std: 0.015
    paper_value: 0.945
    paper_std: 0.015
    metric: Fidelity
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Amazon dataset
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.945
    true_std: 0.015
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.945
    sort_std: 0.015
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
  - model: Gspell+
    model_key: gspell+
    model_plain: Gspell+
    value: 0.92
    std: 0.018
    paper_value: 0.92
    paper_std: 0.018
    metric: Fidelity
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Amazon dataset
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.92
    true_std: 0.018
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.92
    sort_std: 0.018
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.91
    std: 0.011
    paper_value: 0.91
    paper_std: 0.011
    metric: Fidelity
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Amazon dataset
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.91
    true_std: 0.011
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.91
    sort_std: 0.011
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
  - model: LLM
    model_key: llm
    model_plain: LLM
    value: 0.86
    std: 0.012
    paper_value: 0.86
    paper_std: 0.012
    metric: Fidelity
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Amazon dataset
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86
    true_std: 0.012
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.012
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
  - model: PGExplainer
    model_key: pgexplainer
    model_plain: PGExplainer
    value: 0.738
    std: 0.056
    paper_value: 0.738
    paper_std: 0.056
    metric: Fidelity
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Amazon dataset
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.738
    true_std: 0.056
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.738
    sort_std: 0.056
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
  - model: Node
    model_key: node
    model_plain: Node
    value: 0.678
    std: 0.027
    paper_value: 0.678
    paper_std: 0.027
    metric: Fidelity
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Amazon dataset
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.678
    true_std: 0.027
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.678
    sort_std: 0.027
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
  - model: TAGExplainer
    model_key: tagexplainer
    model_plain: TAGExplainer
    value: 0.651
    std: 0.044
    paper_value: 0.651
    paper_std: 0.044
    metric: Fidelity
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Amazon dataset
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.651
    true_std: 0.044
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.651
    sort_std: 0.044
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
  rank_metric: Fidelity
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Fidelity
  metric: Fidelity
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: WikiCS
  rows:
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    value: 0.99
    std: 0.0
    paper_value: 0.99
    paper_std: 0.0
    metric: Fidelity
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
    protocol_note: Node classification task on WikiCS using Fidelity metric.
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.99
    true_std: 0.0
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.99
    sort_std: 0.0
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
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.933
    std: 0.0
    paper_value: 0.933
    paper_std: 0.0
    metric: Fidelity
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
    protocol_note: Node classification task on WikiCS using Fidelity metric.
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.933
    true_std: 0.0
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.0
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
  - model: LLM
    model_key: llm
    model_plain: LLM
    value: 0.914
    std: 0.01
    paper_value: 0.914
    paper_std: 0.01
    metric: Fidelity
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
    protocol_note: Node classification task on WikiCS using Fidelity metric.
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.914
    true_std: 0.01
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.914
    sort_std: 0.01
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
  - model: PGExplainer
    model_key: pgexplainer
    model_plain: PGExplainer
    value: 0.906
    std: 0.0
    paper_value: 0.906
    paper_std: 0.0
    metric: Fidelity
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
    protocol_note: Node classification task on WikiCS using Fidelity metric.
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.906
    true_std: 0.0
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.906
    sort_std: 0.0
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
  - model: Gspell+
    model_key: gspell+
    model_plain: Gspell+
    value: 0.865
    std: 0.0
    paper_value: 0.865
    paper_std: 0.0
    metric: Fidelity
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on WikiCS using Fidelity metric.
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.865
    true_std: 0.0
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.865
    sort_std: 0.0
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
  - model: TAGExplainer
    model_key: tagexplainer
    model_plain: TAGExplainer
    value: 0.764
    std: 0.011
    paper_value: 0.764
    paper_std: 0.011
    metric: Fidelity
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
    protocol_note: Node classification task on WikiCS using Fidelity metric.
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.764
    true_std: 0.011
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.764
    sort_std: 0.011
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
  - model: Node
    model_key: node
    model_plain: Node
    value: 0.723
    std: 0.0
    paper_value: 0.723
    paper_std: 0.0
    metric: Fidelity
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on WikiCS using Fidelity metric.
    date: Aug 9, 2025
    date_display: Aug 2025
    date_iso: '2025-08-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.723
    true_std: 0.0
    value_gap_source_arxiv: '2508.07117'
    value_gap_source_title: 'From Nodes to Narratives: Explaining Graph Neural Networks
      with LLMs and Graph Context'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.723
    sort_std: 0.0
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
  rank_metric: Fidelity
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Fidelity
  metric: Fidelity
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: Other Graph Benchmarks
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: WikiCS
      dataset_slug: wikics
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
single_proposed_model: Gspell+
main_figure: /figures/2508.07117/main_figure.jpegoptim.jpg
---

