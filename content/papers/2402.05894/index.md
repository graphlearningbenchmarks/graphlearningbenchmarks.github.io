---
title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
arxiv_id: '2402.05894'
source_url: ''
authors:
- name: Shengxiang Hu
  orcid: null
  s2_author_id: '2122825801'
  s2_url: null
- name: Guobing Zou
  orcid: null
  s2_author_id: '143896764'
  s2_url: null
- name: Song Yang
  orcid: null
  s2_author_id: '2283509751'
  s2_url: null
- name: Yanglan Gan
  orcid: null
  s2_author_id: '1751935'
  s2_url: null
- name: Bofeng Zhang
  orcid: null
  s2_author_id: '2243445819'
  s2_url: null
- name: Yixin Chen
  orcid: null
  s2_author_id: '2116664622'
  s2_url: null
published_date: Feb 8, 2024
published_date_iso: '2024-02-08'
published_venue: AAAI 2024
published_conference: AAAI 2024
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Recent advancements in leveraging Large Language Models (LLMs) for Text-Attributed
  Graphs (TAGs) learning have shown significant potential, but practical deployment
  is often hindered by substantial computational and storage demands. Conventional
  Graph Neural Networks (GNNs) are more efficient but struggle with the intricate
  semantics embedded in TAGs. To combine the semantic understanding of LLMs with the
  efficiency of GNNs, we propose a novel LLM-to-GNN knowledge distillation framework,
  istic raph nowledge istillation (LinguGKD), which employs TAG-oriented instruction
  tuning to train pre-trained LLMs as teachers and introduces a layer-adaptive contrastive
  distillation strategy to align node features between teacher LLMs and student GNNs
  within a latent space, effectively transferring the semantic and complex relational
  understanding from LLMs to GNNs. Extensive experiments across various LLM and GNN
  architectures on multiple datasets demonstrate that LinguGKD significantly enhances
  the predictive accuracy and convergence rate of GNNs without requiring additional
  training data or model parameters. Compared to teacher LLMs, the distilled GNNs
  offer superior inference speed and reduced resource requirements, making them highly
  practical for deployment in resource-constrained environments. Furthermore, our
  framework demonstrates significant potential for leveraging ongoing advancements
  in LLM research to continuously improve GNN performance.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Cora
  is_multi_metric: true
  rows:
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    metric_values:
    - 0.9635
    - null
    metric_stds:
    - 0.0019
    - null
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
    published_venue: ''
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9635
    sort_std: 0.0019
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
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    metric_values:
    - 0.9629
    - null
    metric_stds:
    - 0.0015
    - null
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
    published_venue: ''
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.9629
    sort_std: 0.0015
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
  - model: Coral
    model_key: coral
    model_plain: Coral
    metric_values:
    - 0.9574
    - null
    metric_stds:
    - 0.0039
    - null
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
    published_venue: ''
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.9574
    sort_std: 0.0039
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
  - model: GraphSAGE_(Llama3)
    model_key: graphsage_(llama3)
    model_plain: GraphSAGE_(Llama3)
    metric_values:
    - 0.917
    - null
    metric_stds:
    - 0.0051
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.917
    sort_std: 0.0051
    true_value: 0.917
    true_std: 0.0051
    paper_value: 0.917
    paper_std: 0.0051
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: distilled from the corresponding teacher LLMs indicated
      by the subscripts
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 26
  - model: GAT_(Llama3)
    model_key: gat_(llama3)
    model_plain: GAT_(Llama3)
    metric_values:
    - 0.9151
    - null
    metric_stds:
    - 0.0035
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9151
    sort_std: 0.0035
    true_value: 0.9151
    true_std: 0.0035
    paper_value: 0.9151
    paper_std: 0.0035
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: distilled from the corresponding teacher LLMs indicated
      by the subscripts
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 27
  - model: LinguGraph-Llama3 (8B)
    model_key: lingugraph-llama3 (8b)
    model_plain: LinguGraph-Llama3 (8B)
    metric_values:
    - 0.9151
    - null
    metric_stds:
    - 0.0046
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 8.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.9151
    sort_std: 0.0046
    true_value: 0.9151
    true_std: 0.0046
    paper_value: 0.9151
    paper_std: 0.0046
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: LinguGraph-Llama3 (8B) represents teacher LLMs obtained
      by fine-tuning different PLMs
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 28
  - model: GIN_(Llama3)
    model_key: gin_(llama3)
    model_plain: GIN_(Llama3)
    metric_values:
    - 0.9133
    - null
    metric_stds:
    - 0.0028
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9133
    sort_std: 0.0028
    true_value: 0.9133
    true_std: 0.0028
    paper_value: 0.9133
    paper_std: 0.0028
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: distilled from the corresponding teacher LLMs indicated
      by the subscripts
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 31
  - model: GCN_(Llama3)
    model_key: gcn_(llama3)
    model_plain: GCN_(Llama3)
    metric_values:
    - 0.9077
    - null
    metric_stds:
    - 0.0028
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9077
    sort_std: 0.0028
    true_value: 0.9077
    true_std: 0.0028
    paper_value: 0.9077
    paper_std: 0.0028
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: distilled from the corresponding teacher LLMs indicated
      by the subscripts
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 36
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.8653
    - 0.8566
    metric_stds:
    - 0.0092
    - 0.0078
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9004
    sort_std: null
    true_value: 0.9004
    true_std: null
    paper_value: 0.8653
    paper_std: 0.0092
    has_value_gap: true
    has_value_note: false
    value_gap: 0.03510000000000002
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_note: ''
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.03510000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
    global_rank: 42
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    metric_values:
    - 0.8852
    - 0.8796
    metric_stds:
    - 0.0095
    - 0.0085
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8976
    sort_std: 0.016
    true_value: 0.8976
    true_std: 0.016
    paper_value: 0.8852
    paper_std: 0.0095
    has_value_gap: true
    has_value_note: false
    value_gap: 0.012399999999999967
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_note: ''
    at_pub_value: 0.8976
    at_pub_std: 0.016
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.012399999999999967
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 50
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    metric_values:
    - 0.8975
    - 0.8894
    metric_stds:
    - 0.0116
    - 0.0054
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8975
    sort_std: 0.0116
    true_value: 0.8975
    true_std: 0.0116
    paper_value: 0.8975
    paper_std: 0.0116
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: 0.8975
    at_pub_std: 0.0116
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 51
  - model: RevGAT
    model_key: revgat
    model_plain: RevGAT
    metric_values:
    - 0.8911
    - 0.8765
    metric_stds:
    - 0.0
    - 0.0058
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8911
    sort_std: 0.001
    true_value: 0.8911
    true_std: 0.001
    paper_value: 0.8911
    paper_std: 0.0
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_note: ''
    at_pub_value: 0.8911
    at_pub_std: 0.0
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
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
    arxiv_id: ''
    title: ''
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 76
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.8911
    - null
    metric_stds:
    - 0.0012
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    published_venue: ''
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 75
    is_best: false
    sort_value: 0.8911
    sort_std: 0.0012
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.8612
    - 0.8505
    metric_stds:
    - 0.0095
    - 0.0088
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8897
    sort_std: null
    true_value: 0.8897
    true_std: null
    paper_value: 0.8612
    paper_std: 0.0095
    has_value_gap: true
    has_value_note: false
    value_gap: 0.02850000000000008
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_note: ''
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.027800000000000047
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
    global_rank: 81
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    metric_values:
    - 0.8893
    - 0.8758
    metric_stds:
    - 0.0137
    - 0.0071
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8893
    sort_std: 0.0137
    true_value: 0.8893
    true_std: 0.0137
    paper_value: 0.8893
    paper_std: 0.0137
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: 0.8893
    at_pub_std: 0.0137
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 83
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - 0.8708
    - 0.8596
    metric_stds:
    - 0.0085
    - 0.0073
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8889
    sort_std: null
    true_value: 0.8889
    true_std: null
    paper_value: 0.8708
    paper_std: 0.0085
    has_value_gap: true
    has_value_note: false
    value_gap: 0.018100000000000005
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_note: ''
    at_pub_value: 0.8777
    at_pub_std: 0.0183
    at_pub_source_arxiv: '2110.15777'
    at_pub_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.006900000000000017
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 88
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    metric_values:
    - 0.8885
    - 0.8792
    metric_stds:
    - 0.0136
    - 0.0065
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8885
    sort_std: 0.0136
    true_value: 0.8885
    true_std: 0.0136
    paper_value: 0.8885
    paper_std: 0.0136
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: 0.8885
    at_pub_std: 0.0136
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 90
  - model: LinguGraph-Llama2 (7B)
    model_key: lingugraph-llama2 (7b)
    model_plain: LinguGraph-Llama2 (7B)
    metric_values:
    - 0.8819
    - null
    metric_stds:
    - 0.0083
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.8819
    sort_std: 0.0083
    true_value: 0.8819
    true_std: 0.0083
    paper_value: 0.8819
    paper_std: 0.0083
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: LinguGraph-Llama2 (7B) represents teacher LLMs obtained
      by fine-tuning different PLMs
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 135
  - model: LinguGraph-Mistral (7B)
    model_key: lingugraph-mistral (7b)
    model_plain: LinguGraph-Mistral (7B)
    metric_values:
    - 0.8782
    - null
    metric_stds:
    - 0.0088
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.8782
    sort_std: 0.0088
    true_value: 0.8782
    true_std: 0.0088
    paper_value: 0.8782
    paper_std: 0.0088
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: LinguGraph-Mistral (7B) represents teacher LLMs obtained
      by fine-tuning different PLMs
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 162
  - model: GIN
    model_key: gin
    model_plain: GIN
    metric_values:
    - 0.866
    - 0.8537
    metric_stds:
    - 0.0091
    - 0.0074
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.866
    sort_std: 0.0091
    true_value: 0.866
    true_std: 0.0091
    paper_value: 0.866
    paper_std: 0.0091
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: 0.8193
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2110.15777'
    at_pub_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.046699999999999964
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    comparison_source_arxiv: '2110.15777'
    is_best: false
    is_std_outlier: false
    global_rank: 238
  - model: Graphtransformer
    model_key: graphtransformer
    model_plain: Graphtransformer
    metric_values:
    - 0.8642
    - 0.8596
    metric_stds:
    - 0.0082
    - 0.0067
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.8642
    sort_std: 0.0082
    true_value: 0.8642
    true_std: 0.0082
    paper_value: 0.8642
    paper_std: 0.0082
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 250
  - model: SGC-v2
    model_key: sgc-v2
    model_plain: SGC-v2
    metric_values:
    - 0.8548
    - 0.8504
    metric_stds:
    - 0.0148
    - 0.0069
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8548
    sort_std: 0.0148
    true_value: 0.8548
    true_std: 0.0148
    paper_value: 0.8548
    paper_std: 0.0148
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: 0.8548
    at_pub_std: 0.0148
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 301
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    metric_values:
    - 0.8041
    - 0.7998
    metric_stds:
    - 0.003
    - 0.0056
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.8041
    sort_std: 0.002
    true_value: 0.8041
    true_std: 0.002
    paper_value: 0.8041
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_note: ''
    at_pub_value: 0.8041
    at_pub_std: 0.003
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
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
    arxiv_id: ''
    title: ''
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 772
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.7768
    - null
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    published_venue: ''
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 853
    is_best: false
    sort_value: 0.7768
    sort_std: null
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
  - model: Llama3 (8B)
    model_key: llama3 (8b)
    model_plain: Llama3 (8B)
    metric_values:
    - 0.1492
    - null
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 8.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.1492
    sort_std: null
    true_value: 0.1492
    true_std: null
    paper_value: 0.1492
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 1092
  - model: Llama2 (7B)
    model_key: llama2 (7b)
    model_plain: Llama2 (7B)
    metric_values:
    - 0.0923
    - null
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.0923
    sort_std: null
    true_value: 0.0923
    true_std: null
    paper_value: 0.0923
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 1093
  - model: Mistral (7B)
    model_key: mistral (7b)
    model_plain: Mistral (7B)
    metric_values:
    - 0.0876
    - null
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.0876
    sort_std: null
    true_value: 0.0876
    true_std: null
    paper_value: 0.0876
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
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
    published_venue: AAAI 2024
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 1094
  metrics:
  - Accuracy
  - F1
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - F1
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
main_figure: /figures/2402.05894/main_figure.jpegoptim.jpg
---

