---
title: Edge Prompt Tuning for Graph Neural Networks
arxiv_id: '2503.00750'
source_url: ''
authors:
- name: Xingbo Fu
  orcid: null
  s2_author_id: '2194727743'
  s2_url: null
- name: Yinhan He
  orcid: null
  s2_author_id: '2302556971'
  s2_url: null
- name: Jundong Li
  orcid: null
  s2_author_id: '2276482171'
  s2_url: null
published_date: Mar 2, 2025
published_date_iso: '2025-03-02'
published_venue: ICLR 2025
published_conference: ICLR 2025
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Pre-training powerful Graph Neural Networks (GNNs) with unlabeled graph
  data in a self-supervised manner has emerged as a prominent technique in recent
  years. However, inevitable objective gaps often exist between pre-training and downstream
  tasks. To bridge this gap, graph prompt tuning techniques design and learn graph
  prompts by manipulating input graphs or reframing downstream tasks as pre-training
  tasks without fine-tuning the pre-trained GNN models. While recent graph prompt
  tuning methods have proven effective in adapting pre-trained GNN models for downstream
  tasks, they overlook the crucial role of edges in graph prompt design, which can
  significantly affect the quality of graph representations for downstream tasks.
  In this study, we propose EdgePrompt, a simple yet effective graph prompt tuning
  method from the perspective of edges. Unlike previous studies that design prompt
  vectors on node features, EdgePrompt manipulates input graphs by learning additional
  prompt vectors for edges and incorporates the edge prompts through message passing
  in the pre-trained GNN models to better embed graph structural information for downstream
  tasks. Our method is compatible with prevalent GNN architectures pre-trained under
  various pre-training strategies and is universal for different downstream tasks.
  We provide comprehensive theoretical analyses of our method regarding its capability
  of handling node classification and graph classification as downstream tasks. Extensive
  experiments on ten graph datasets under four pre-training strategies demonstrate
  the superiority of our proposed method against six baselines. Our code is available
  at.
codebase_url: https://github.com/xbfu/EdgePrompt
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- EdgePrompt+
mrr: 0.002
adjusted_mrr: 0.002
mrr_dataset_count: 5
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: ENZYMES
  rows:
  - model: 3WLGNN
    model_key: msa-aud
    model_plain: 3WLGNN
    value: 0.892
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2312.10943'
    title: Model Stealing Attack against Graph Classification with Authenticity, Uncertainty
      and Diversity
    date: Dec 18, 2023
    date_display: Dec 2023
    date_iso: '2023-12-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.892
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: 3WLGNN
    model_key: msa-ad
    model_plain: 3WLGNN
    value: 0.89
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.10943'
    title: Model Stealing Attack against Graph Classification with Authenticity, Uncertainty
      and Diversity
    date: Dec 18, 2023
    date_display: Dec 2023
    date_iso: '2023-12-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.89
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3WLGNN
    model_key: msa-au
    model_plain: 3WLGNN
    value: 0.854
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.10943'
    title: Model Stealing Attack against Graph Classification with Authenticity, Uncertainty
      and Diversity
    date: Dec 18, 2023
    date_display: Dec 2023
    date_iso: '2023-12-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.854
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: edgeprompt+
    model_plain: EdgePrompt+
    value: 0.34
    std: 0.0125
    paper_value: 0.34
    paper_std: 0.0125
    metric: Accuracy
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.34
    true_std: 0.0125
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.34
    sort_std: 0.0125
    global_rank: 225
    paper_rank: 225
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Classifier Only
    model_key: classifier only
    model_plain: Classifier Only
    value: 0.3133
    std: 0.0322
    paper_value: 0.3133
    paper_std: 0.0322
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3133
    true_std: 0.0322
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3133
    sort_std: 0.0322
    global_rank: 234
    paper_rank: 234
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPF-plus
    model_key: gpf-plus
    model_plain: GPF-plus
    value: 0.31
    std: 0.015
    paper_value: 0.31
    paper_std: 0.015
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.2292
    at_pub_std: 0.0164
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.08080000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.31
    true_std: 0.015
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.31
    sort_std: 0.015
    global_rank: 236
    paper_rank: 236
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    comparison_source_arxiv: '2406.05346'
    is_best: false
    is_std_outlier: false
  - model: GPF
    model_key: gpf
    model_plain: GPF
    value: 0.3093
    std: 0.0176
    paper_value: 0.3093
    paper_std: 0.0176
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.22
    at_pub_std: 0.0125
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.08930000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3093
    true_std: 0.0176
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3093
    sort_std: 0.0176
    global_rank: 237
    paper_rank: 237
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    comparison_source_arxiv: '2406.05346'
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 0.302
    std: 0.0193
    paper_value: 0.302
    paper_std: 0.0193
    metric: Accuracy
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.2567
    at_pub_std: 0.0349
    at_pub_source_arxiv: '2501.15142'
    at_pub_source_title: 'DAGPrompT: Pushing the Limits of Graph Prompting with a
      Distribution-aware Graph Prompt Tuning Approach'
    at_pub_source_date_iso: '2025-01-25'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.04530000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.302
    true_std: 0.0193
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.302
    sort_std: 0.0193
    global_rank: 242
    paper_rank: 242
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: All-In-One
    model_key: all-in-one
    model_plain: All-In-One
    value: 0.2907
    std: 0.0116
    paper_value: 0.2907
    paper_std: 0.0116
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.2608
    at_pub_std: 0.0486
    at_pub_source_arxiv: '2501.15142'
    at_pub_source_title: 'DAGPrompT: Pushing the Limits of Graph Prompting with a
      Distribution-aware Graph Prompt Tuning Approach'
    at_pub_source_date_iso: '2025-01-25'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.029900000000000038
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2907
    true_std: 0.0116
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2907
    sort_std: 0.0116
    global_rank: 247
    paper_rank: 247
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
  dataset: NCI1
  rows:
  - model: Diverse B12C3
    model_key: msa-aud
    model_plain: Diverse B12C3
    value: 0.969
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2312.10943'
    title: Model Stealing Attack against Graph Classification with Authenticity, Uncertainty
      and Diversity
    date: Dec 18, 2023
    date_display: Dec 2023
    date_iso: '2023-12-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.969
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Diverse B12C3
    model_key: msa-au
    model_plain: Diverse B12C3
    value: 0.966
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.10943'
    title: Model Stealing Attack against Graph Classification with Authenticity, Uncertainty
      and Diversity
    date: Dec 18, 2023
    date_display: Dec 2023
    date_iso: '2023-12-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Diverse B12C3
    model_key: msa-ad
    model_plain: Diverse B12C3
    value: 0.963
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.10943'
    title: Model Stealing Attack against Graph Classification with Authenticity, Uncertainty
      and Diversity
    date: Dec 18, 2023
    date_display: Dec 2023
    date_iso: '2023-12-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.963
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: edgeprompt+
    model_plain: EdgePrompt+
    value: 0.6707
    std: 0.0196
    paper_value: 0.6707
    paper_std: 0.0196
    metric: Accuracy
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6707
    true_std: 0.0196
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6707
    sort_std: 0.0196
    global_rank: 511
    paper_rank: 511
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPF-plus
    model_key: gpf-plus
    model_plain: GPF-plus
    value: 0.6456
    std: 0.011
    paper_value: 0.6456
    paper_std: 0.011
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6456
    true_std: 0.011
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6456
    sort_std: 0.011
    global_rank: 529
    paper_rank: 529
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
    value: 0.6319
    std: 0.0171
    paper_value: 0.6319
    paper_std: 0.0171
    metric: Accuracy
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6319
    true_std: 0.0171
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6319
    sort_std: 0.0171
    global_rank: 535
    paper_rank: 535
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPF
    model_key: gpf
    model_plain: GPF
    value: 0.6266
    std: 0.0183
    paper_value: 0.6266
    paper_std: 0.0183
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6266
    true_std: 0.0183
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6266
    sort_std: 0.0183
    global_rank: 536
    paper_rank: 536
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Classifier Only
    model_key: classifier only
    model_plain: Classifier Only
    value: 0.6249
    std: 0.0195
    paper_value: 0.6249
    paper_std: 0.0195
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6249
    true_std: 0.0195
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6249
    sort_std: 0.0195
    global_rank: 539
    paper_rank: 539
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: All-In-One
    model_key: all-in-one
    model_plain: All-In-One
    value: 0.5914
    std: 0.0212
    paper_value: 0.5914
    paper_std: 0.0212
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 50-shot graph classification
    date: Mar 2, 2025
    date_display: Mar 2025
    date_iso: '2025-03-02'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-03-02'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5914
    true_std: 0.0212
    value_gap_source_arxiv: '2503.00750'
    value_gap_source_title: Edge Prompt Tuning for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5914
    sort_std: 0.0212
    global_rank: 554
    paper_rank: 554
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
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: NCI1
      dataset_slug: nci1
    - dataset: ENZYMES
      dataset_slug: enzymes
single_proposed_model: EdgePrompt+
---

