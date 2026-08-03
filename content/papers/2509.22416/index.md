---
title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained Models'
arxiv_id: '2509.22416'
source_url: ''
authors:
- name: Yongqi Huang
  orcid: null
  s2_author_id: '2293653375'
  s2_url: null
- name: Jitao Zhao
  orcid: null
  s2_author_id: '2230259009'
  s2_url: null
- name: Dongxiao He
  orcid: null
  s2_author_id: '2258959961'
  s2_url: null
- name: Xiaobao Wang
  orcid: null
  s2_author_id: '2108114840'
  s2_url: null
- name: Yawen Li
  orcid: null
  s2_author_id: '2222317038'
  s2_url: null
- name: Yuxiao Huang
  orcid: null
  s2_author_id: '2108728683'
  s2_url: null
- name: Di Jin
  orcid: null
  s2_author_id: '2288101014'
  s2_url: null
- name: Zhiyong Feng
  orcid: null
  s2_author_id: '2287699649'
  s2_url: null
published_date: Sep 26, 2025
published_date_iso: '2025-09-26'
published_venue: NeurIPS 2025
published_conference: NeurIPS 2025
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: 'Graph Prompt Learning (GPL) has emerged as a promising paradigm that bridges
  graph pretraining models and downstream scenarios, mitigating label dependency and
  the misalignment between upstream pretraining and downstream tasks. Although existing
  GPL studies explore various prompt strategies, their effectiveness and underlying
  principles remain unclear. We identify two critical limitations: (1) Lack of consensus
  on underlying mechanisms: Despite current GPLs have advanced the field, there is
  no consensus on how prompts interact with pretrained models, as different strategies
  intervene at varying spaces within the model, i.e., input-level, layer-wise, and
  representation-level prompts. (2) Limited scenario adaptability: Most methods fail
  to generalize across diverse downstream scenarios, especially under data distribution
  shifts (e.g., homophilic-to-heterophilic graphs). To address these issues, we theoretically
  analyze existing GPL approaches and reveal that representation-level prompts essentially
  function as fine-tuning a simple downstream classifier, proposing that graph prompt
  learning should focus on unleashing the capability of pretrained models, and the
  classifier should adapt to downstream scenarios. Based on our findings, we propose
  UniPrompt, a novel GPL method that adapts any pretrained models, unleashing the
  capability of pretrained models while preserving the input graph. Extensive experiments
  demonstrate that our method can effectively integrate with various pretrained models
  and achieve strong performance across in-domain and cross-domain scenarios.'
codebase_url: https://github.com/hedongxiao-tju/UniPrompt
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- UniPrompt
mrr: 0.0022
adjusted_mrr: 0.0022
mrr_dataset_count: 7
benchmark_categories:
- Classic
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 5
  total: 13
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id005
  dataset: Actor
  rows:
  - model: CoCN
    model_key: diggr
    model_plain: CoCN
    value: 0.4535
    std: 0.0353
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_display: Aug 2024
    date_iso: '2024-08-24'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.4535
    sort_std: 0.0353
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CoCN
    model_key: uniaug - polygcl
    model_plain: CoCN
    value: 0.4301
    std: 0.0127
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.01899'
    title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
    date: Jun 4, 2024
    date_display: Jun 2024
    date_iso: '2024-06-04'
    venue: NeurIPS'25
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4301
    sort_std: 0.0127
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CoCN
    model_key: adaptkry
    model_plain: CoCN
    value: 0.427
    std: 0.0114
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.07954'
    title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive Krylov Subspace
      Approach'
    date: Mar 12, 2024
    date_display: Mar 2024
    date_iso: '2024-03-12'
    venue: The Web Conference
    codebase_url: https://github.com/kkhuang81/AdaptKry
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.427
    sort_std: 0.0114
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPF
    model_key: gpf
    model_plain: GPF
    value: 0.2081
    std: 0.0308
    paper_value: 0.2081
    paper_std: 0.0308
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
    protocol_note: 1-shot node classification on Actor using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.287
    at_pub_std: 0.0335
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.07889999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.287
    true_std: 0.0335
    value_gap_source_arxiv: '2406.05346'
    value_gap_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    value_gap_source_is_current_paper: false
    value_gap: 0.07889999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.287
    sort_std: 0.0335
    global_rank: 333
    paper_rank: 432
    rank_delta: 99
    rank_delta_abs: 99
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    comparison_source_arxiv: '2406.05346'
    is_best: false
    is_std_outlier: false
  - model: UniPrompt
    model_key: uniprompt
    model_plain: UniPrompt
    value: 0.2623
    std: 0.0446
    paper_value: 0.2623
    paper_std: 0.0446
    metric: Accuracy
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
    protocol_note: 1-shot node classification on Actor using GRACE pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2623
    true_std: 0.0446
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2623
    sort_std: 0.0446
    global_rank: 369
    paper_rank: 369
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
    value: 0.2108
    std: 0.0217
    paper_value: 0.2108
    paper_std: 0.0217
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
    protocol_note: 1-shot node classification on Actor using GraphMAE pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.2461
    at_pub_std: 0.028
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.035300000000000026
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.2461
    true_std: 0.028
    value_gap_source_arxiv: '2406.05346'
    value_gap_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    value_gap_source_is_current_paper: false
    value_gap: 0.035300000000000026
    has_value_note: false
    value_note: ''
    sort_value: 0.2461
    sort_std: 0.028
    global_rank: 391
    paper_rank: 431
    rank_delta: 40
    rank_delta_abs: 40
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPPT
    model_key: gppt
    model_plain: GPPT
    value: 0.1981
    std: 0.0163
    paper_value: 0.1981
    paper_std: 0.0163
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
    protocol_note: 1-shot node classification on Actor using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.2258
    at_pub_std: 0.0197
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.027700000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.2258
    true_std: 0.0197
    value_gap_source_arxiv: '2406.05346'
    value_gap_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    value_gap_source_is_current_paper: false
    value_gap: 0.027700000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.2258
    sort_std: 0.0197
    global_rank: 414
    paper_rank: 439
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Fine-tune
    model_key: fine-tune
    model_plain: Fine-tune
    value: 0.2136
    std: 0.0328
    paper_value: 0.2136
    paper_std: 0.0328
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
    protocol_note: 1-shot node classification on Actor using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2136
    true_std: 0.0328
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2136
    sort_std: 0.0328
    global_rank: 429
    paper_rank: 429
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: edgeprompt+
    model_plain: EdgePrompt+
    value: 0.2136
    std: 0.0276
    paper_value: 0.2136
    paper_std: 0.0276
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
    protocol_note: 1-shot node classification on Actor using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2136
    true_std: 0.0276
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2136
    sort_std: 0.0276
    global_rank: 430
    paper_rank: 430
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Linear-probe
    model_key: linear-probe
    model_plain: Linear-probe
    value: 0.2133
    std: 0.0262
    paper_value: 0.2133
    paper_std: 0.0262
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
    protocol_note: 1-shot node classification on Actor using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2133
    true_std: 0.0262
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2133
    sort_std: 0.0262
    global_rank: 431
    paper_rank: 431
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
    value: 0.1984
    std: 0.0279
    paper_value: 0.1984
    paper_std: 0.0279
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification on Actor using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1984
    true_std: 0.0279
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1984
    sort_std: 0.0279
    global_rank: 439
    paper_rank: 439
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
- &id006
  dataset: Chameleon
  rows:
  - model: Random
    model_key: hetero-s (gat 8-layer)
    model_plain: Random
    value: 0.8693
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
    arxiv_id: '2406.12539'
    title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
      Heterophilic Graphs'
    date: Jun 18, 2024
    date_display: Jun 2024
    date_iso: '2024-06-18'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/bingreeky/HeteroSnoH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8693
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Random
    model_key: trans.conv+cna
    model_plain: Random
    value: 0.8586
    std: 0.018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8586
    sort_std: 0.018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Random
    model_key: gat
    model_plain: Random
    value: 0.856
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
    arxiv_id: '2406.12539'
    title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
      Heterophilic Graphs'
    date: Jun 18, 2024
    date_display: Jun 2024
    date_iso: '2024-06-18'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/bingreeky/HeteroSnoH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.856
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 0.2828
    std: 0.0438
    paper_value: 0.2828
    paper_std: 0.0438
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification using GRACE pretraining; Chameleon is
      a heterophilic dataset.
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.2536
    at_pub_std: 0.0399
    at_pub_source_arxiv: '2502.08092'
    at_pub_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    at_pub_source_date_iso: '2025-02-12'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.029200000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2828
    true_std: 0.0438
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2828
    sort_std: 0.0438
    global_rank: 298
    paper_rank: 298
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniPrompt
    model_key: uniprompt
    model_plain: UniPrompt
    value: 0.2667
    std: 0.0251
    paper_value: 0.2667
    paper_std: 0.0251
    metric: Accuracy
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
    protocol_note: 1-shot node classification using GRACE pretraining; Chameleon is
      a heterophilic dataset.
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2667
    true_std: 0.0251
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2667
    sort_std: 0.0251
    global_rank: 302
    paper_rank: 302
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Fine-tune
    model_key: fine-tune
    model_plain: Fine-tune
    value: 0.2622
    std: 0.0273
    paper_value: 0.2622
    paper_std: 0.0273
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
    protocol_note: 1-shot node classification using GRACE pretraining; Chameleon is
      a heterophilic dataset.
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2622
    true_std: 0.0273
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2622
    sort_std: 0.0273
    global_rank: 303
    paper_rank: 303
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
    value: 0.2603
    std: 0.0437
    paper_value: 0.2603
    paper_std: 0.0437
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
    protocol_note: 1-shot node classification using GRACE pretraining; Chameleon is
      a heterophilic dataset.
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.2612
    at_pub_std: 0.0375
    at_pub_source_arxiv: '2502.08092'
    at_pub_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    at_pub_source_date_iso: '2025-02-12'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-02-12'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.0009000000000000119
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.2612
    true_std: 0.0375
    value_gap_source_arxiv: '2502.08092'
    value_gap_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.0009000000000000119
    has_value_note: false
    value_note: ''
    sort_value: 0.2612
    sort_std: 0.0375
    global_rank: 304
    paper_rank: 304
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPPT
    model_key: gppt
    model_plain: GPPT
    value: 0.2546
    std: 0.0543
    paper_value: 0.2546
    paper_std: 0.0543
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
    protocol_note: 1-shot node classification using GRACE pretraining; Chameleon is
      a heterophilic dataset.
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2546
    true_std: 0.0543
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2546
    sort_std: 0.0543
    global_rank: 306
    paper_rank: 306
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Linear-probe
    model_key: linear-probe
    model_plain: Linear-probe
    value: 0.2427
    std: 0.0384
    paper_value: 0.2427
    paper_std: 0.0384
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
    protocol_note: 1-shot node classification using GRACE pretraining; Chameleon is
      a heterophilic dataset.
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2427
    true_std: 0.0384
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2427
    sort_std: 0.0384
    global_rank: 308
    paper_rank: 308
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: edgeprompt+
    model_plain: EdgePrompt+
    value: 0.2379
    std: 0.0331
    paper_value: 0.2379
    paper_std: 0.0331
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
    protocol_note: 1-shot node classification using GRACE pretraining; Chameleon is
      a heterophilic dataset.
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2379
    true_std: 0.0331
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2379
    sort_std: 0.0331
    global_rank: 309
    paper_rank: 309
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
    value: 0.2241
    std: 0.0358
    paper_value: 0.2241
    paper_std: 0.0358
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
    protocol_note: 1-shot node classification using DGI pretraining; Chameleon is
      a heterophilic dataset.
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2241
    true_std: 0.0358
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2241
    sort_std: 0.0358
    global_rank: 311
    paper_rank: 311
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
- &id002
  dataset: CiteSeer
  rows:
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: cna
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.9575
    std: 0.0058
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9575
    sort_std: 0.0058
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: is-gib
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.939
    std: 0.0187
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.939
    sort_std: 0.0187
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: eerm
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.9112
    std: 0.0145
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9112
    sort_std: 0.0145
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPPT
    model_key: gppt
    model_plain: GPPT
    value: 0.3742
    std: 0.091
    paper_value: 0.3742
    paper_std: 0.091
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
    protocol_note: 1-shot node classification using GRACE pretraining; Planetoid split
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.7031
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2407.11361'
    at_pub_source_title: 'Graph Structure Prompt Learning: A Novel Methodology to
      Improve Performance of Graph Neural Networks'
    at_pub_source_date_iso: '2024-07-16'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.32889999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7031
    true_std: 0.0039
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.32889999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7031
    sort_std: 0.0039
    global_rank: 588
    paper_rank: 843
    rank_delta: 255
    rank_delta_abs: 255
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    comparison_source_arxiv: '2407.11361'
    is_best: false
    is_std_outlier: false
  - model: UniPrompt
    model_key: uniprompt
    model_plain: UniPrompt
    value: 0.4929
    std: 0.112
    paper_value: 0.4929
    paper_std: 0.112
    metric: Accuracy
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
    protocol_note: 1-shot node classification using GraphMAE pretraining; Planetoid
      split
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4929
    true_std: 0.112
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4929
    sort_std: 0.112
    global_rank: 825
    paper_rank: 825
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Linear-probe
    model_key: linear-probe
    model_plain: Linear-probe
    value: 0.4808
    std: 0.0696
    paper_value: 0.4808
    paper_std: 0.0696
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
    protocol_note: 1-shot node classification using GraphMAE pretraining; Planetoid
      split
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4808
    true_std: 0.0696
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4808
    sort_std: 0.0696
    global_rank: 826
    paper_rank: 826
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Fine-tune
    model_key: fine-tune
    model_plain: Fine-tune
    value: 0.4616
    std: 0.063
    paper_value: 0.4616
    paper_std: 0.063
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
    protocol_note: 1-shot node classification using GRACE pretraining; Planetoid split
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4616
    true_std: 0.063
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4616
    sort_std: 0.063
    global_rank: 829
    paper_rank: 829
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
    value: 0.4398
    std: 0.0761
    paper_value: 0.4398
    paper_std: 0.0761
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification using DGI pretraining; Planetoid split
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.4534
    at_pub_std: 0.1053
    at_pub_source_arxiv: '2502.08092'
    at_pub_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    at_pub_source_date_iso: '2025-02-12'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-02-12'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.013600000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4534
    true_std: 0.1053
    value_gap_source_arxiv: '2502.08092'
    value_gap_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.013600000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.4534
    sort_std: 0.1053
    global_rank: 831
    paper_rank: 838
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPF
    model_key: gpf
    model_plain: GPF
    value: 0.4489
    std: 0.0661
    paper_value: 0.4489
    paper_std: 0.0661
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
    protocol_note: 1-shot node classification using DGI pretraining; Planetoid split
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.4328
    at_pub_std: 0.0882
    at_pub_source_arxiv: '2502.08092'
    at_pub_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    at_pub_source_date_iso: '2025-02-12'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.016100000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4489
    true_std: 0.0661
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4489
    sort_std: 0.0661
    global_rank: 835
    paper_rank: 835
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
    value: 0.3172
    std: 0.0278
    paper_value: 0.3172
    paper_std: 0.0278
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
    protocol_note: 1-shot node classification using GraphMAE pretraining; Planetoid
      split
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.4041
    at_pub_std: 0.028
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.08690000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4041
    true_std: 0.028
    value_gap_source_arxiv: '2406.05346'
    value_gap_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    value_gap_source_is_current_paper: false
    value_gap: 0.08690000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.4041
    sort_std: 0.028
    global_rank: 841
    paper_rank: 848
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    comparison_source_arxiv: '2406.05346'
    is_best: false
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: edgeprompt+
    model_plain: EdgePrompt+
    value: 0.3854
    std: 0.0637
    paper_value: 0.3854
    paper_std: 0.0637
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
    protocol_note: 1-shot node classification using DGI pretraining; Planetoid split
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3854
    true_std: 0.0637
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3854
    sort_std: 0.0637
    global_rank: 843
    paper_rank: 843
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
- &id001
  dataset: Cora
  rows:
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: exphormer
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
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
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: sgformer
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
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
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: coral
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
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
  - model: GPF
    model_key: gpf
    model_plain: GPF
    value: 0.5168
    std: 0.0952
    paper_value: 0.5168
    paper_std: 0.0952
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
    protocol_note: 1-shot node classification using DGI pretraining; Planetoid split
      (20 per class train split)
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.576
    at_pub_std: 0.1388
    at_pub_source_arxiv: '2502.08092'
    at_pub_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    at_pub_source_date_iso: '2025-02-12'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-02-12'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.05919999999999992
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.576
    true_std: 0.1388
    value_gap_source_arxiv: '2502.08092'
    value_gap_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.05919999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.576
    sort_std: 0.1388
    global_rank: 854
    paper_rank: 866
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 0.5145
    std: 0.0963
    paper_value: 0.5145
    paper_std: 0.0963
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification using GraphMAE pretraining; Planetoid
      split (20 per class train split)
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.5425
    at_pub_std: 0.0938
    at_pub_source_arxiv: '2502.08092'
    at_pub_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    at_pub_source_date_iso: '2025-02-12'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-02-12'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.028000000000000025
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.5425
    true_std: 0.0938
    value_gap_source_arxiv: '2502.08092'
    value_gap_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.028000000000000025
    has_value_note: false
    value_note: ''
    sort_value: 0.5425
    sort_std: 0.0938
    global_rank: 861
    paper_rank: 866
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: All-In-One
    model_key: all-in-one
    model_plain: All-In-One
    value: 0.3453
    std: 0.0586
    paper_value: 0.3453
    paper_std: 0.0586
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
    protocol_note: 1-shot node classification using GRACE pretraining; Planetoid split
      (20 per class train split)
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.5239
    at_pub_std: 0.1017
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.17860000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5239
    true_std: 0.1017
    value_gap_source_arxiv: '2406.05346'
    value_gap_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    value_gap_source_is_current_paper: false
    value_gap: 0.17860000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.5239
    sort_std: 0.1017
    global_rank: 865
    paper_rank: 899
    rank_delta: 34
    rank_delta_abs: 34
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    comparison_source_arxiv: '2406.05346'
    is_best: false
    is_std_outlier: false
  - model: Fine-tune
    model_key: fine-tune
    model_plain: Fine-tune
    value: 0.5022
    std: 0.0928
    paper_value: 0.5022
    paper_std: 0.0928
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
    protocol_note: 1-shot node classification using DGI pretraining; Planetoid split
      (20 per class train split)
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5022
    true_std: 0.0928
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5022
    sort_std: 0.0928
    global_rank: 869
    paper_rank: 869
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Linear-probe
    model_key: linear-probe
    model_plain: Linear-probe
    value: 0.5013
    std: 0.1206
    paper_value: 0.5013
    paper_std: 0.1206
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
    protocol_note: 1-shot node classification using GraphMAE pretraining; Planetoid
      split (20 per class train split)
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5013
    true_std: 0.1206
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5013
    sort_std: 0.1206
    global_rank: 870
    paper_rank: 870
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniPrompt
    model_key: uniprompt
    model_plain: UniPrompt
    value: 0.4995
    std: 0.1048
    paper_value: 0.4995
    paper_std: 0.1048
    metric: Accuracy
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
    protocol_note: 1-shot node classification using DGI pretraining; Planetoid split
      (20 per class train split)
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4995
    true_std: 0.1048
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4995
    sort_std: 0.1048
    global_rank: 871
    paper_rank: 871
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: edgeprompt+
    model_plain: EdgePrompt+
    value: 0.4532
    std: 0.0903
    paper_value: 0.4532
    paper_std: 0.0903
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
    protocol_note: 1-shot node classification using GRACE pretraining; Planetoid split
      (20 per class train split)
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4704
    true_std: 0.0697
    value_gap_source_arxiv: '2604.11257'
    value_gap_source_title: Unified Graph Prompt Learning via Low-Rank Graph Message
      Prompting
    value_gap_source_is_current_paper: false
    value_gap: 0.017199999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.4704
    sort_std: 0.0697
    global_rank: 877
    paper_rank: 884
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPPT
    model_key: gppt
    model_plain: GPPT
    value: 0.4219
    std: 0.0642
    paper_value: 0.4219
    paper_std: 0.0642
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
    protocol_note: 1-shot node classification using GRACE pretraining; Planetoid split
      (20 per class train split)
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.4315
    at_pub_std: 0.0944
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.009599999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4315
    true_std: 0.0944
    value_gap_source_arxiv: '2406.05346'
    value_gap_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    value_gap_source_is_current_paper: false
    value_gap: 0.009599999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.4315
    sort_std: 0.0944
    global_rank: 889
    paper_rank: 889
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: Cornell
  rows:
  - model: Kron
    model_key: p^2gnn
    model_plain: Kron
    value: 0.9541
    std: 0.0272
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9541
    sort_std: 0.0272
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Kron
    model_key: acm-gcn
    model_plain: Kron
    value: 0.948
    std: 0.038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.19785'
    title: Heterophily-informed Message Passing
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/AaltoML/heterophily-imp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.948
    sort_std: 0.038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Kron
    model_key: rf-gcn
    model_plain: Kron
    value: 0.9429
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
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9429
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UniPrompt
    model_key: uniprompt
    model_plain: UniPrompt
    value: 0.528
    std: 0.1108
    paper_value: 0.528
    paper_std: 0.1108
    metric: Accuracy
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
    protocol_note: 1-shot node classification using GRACE pretraining; Geom-GCN 10
      fixed splits
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.528
    true_std: 0.1108
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.528
    sort_std: 0.1108
    global_rank: 455
    paper_rank: 455
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
    value: 0.2891
    std: 0.0885
    paper_value: 0.2891
    paper_std: 0.0885
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
    source_ref: GPF [23]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification using GRACE pretraining; Geom-GCN 10
      fixed splits
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.3817
    at_pub_std: 0.0815
    at_pub_source_arxiv: '2502.02017'
    at_pub_source_title: 'Multi-Domain Graph Foundation Models: Robust Knowledge Transfer
      via Topology Alignment'
    at_pub_source_date_iso: '2025-02-04'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.09259999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.3817
    true_std: 0.0815
    value_gap_source_arxiv: '2502.02017'
    value_gap_source_title: 'Multi-Domain Graph Foundation Models: Robust Knowledge
      Transfer via Topology Alignment'
    value_gap_source_is_current_paper: false
    value_gap: 0.09259999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.3817
    sort_std: 0.0815
    global_rank: 534
    paper_rank: 549
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Fine-tune
    model_key: fine-tune
    model_plain: Fine-tune
    value: 0.3582
    std: 0.113
    paper_value: 0.3582
    paper_std: 0.113
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
    protocol_note: 1-shot node classification using GraphMAE pretraining; Geom-GCN
      10 fixed splits
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3582
    true_std: 0.113
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3582
    sort_std: 0.113
    global_rank: 538
    paper_rank: 538
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPPT
    model_key: gppt
    model_plain: GPPT
    value: 0.2901
    std: 0.0832
    paper_value: 0.2901
    paper_std: 0.0832
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
    source_ref: GPPT [20]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification using DGI pretraining; Geom-GCN 10 fixed
      splits
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.3469
    at_pub_std: 0.0854
    at_pub_source_arxiv: '2502.02017'
    at_pub_source_title: 'Multi-Domain Graph Foundation Models: Robust Knowledge Transfer
      via Topology Alignment'
    at_pub_source_date_iso: '2025-02-04'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2026-05-11'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.05679999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.3568
    true_std: 0.0963
    value_gap_source_arxiv: '2605.09993'
    value_gap_source_title: Learning Graph Foundation Models on Riemannian Graph-of-Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.06669999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.3568
    sort_std: 0.0963
    global_rank: 539
    paper_rank: 549
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Linear-probe
    model_key: linear-probe
    model_plain: Linear-probe
    value: 0.3492
    std: 0.0974
    paper_value: 0.3492
    paper_std: 0.0974
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
    protocol_note: 1-shot node classification using GRACE pretraining; Geom-GCN 10
      fixed splits
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3492
    true_std: 0.0974
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3492
    sort_std: 0.0974
    global_rank: 541
    paper_rank: 541
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
    value: 0.2382
    std: 0.075
    paper_value: 0.2382
    paper_std: 0.075
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
    source_ref: GraphPrompt [21]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification using GraphMAE pretraining; Geom-GCN
      10 fixed splits
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-11'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.3243
    true_std: 0.1081
    value_gap_source_arxiv: '2605.09993'
    value_gap_source_title: Learning Graph Foundation Models on Riemannian Graph-of-Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.08609999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.3243
    sort_std: 0.1081
    global_rank: 544
    paper_rank: 559
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: edgeprompt+
    model_plain: EdgePrompt+
    value: 0.3213
    std: 0.0742
    paper_value: 0.3213
    paper_std: 0.0742
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
    source_ref: EdgePrompt [24]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification using GRACE pretraining; Geom-GCN 10
      fixed splits
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3213
    true_std: 0.0742
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3213
    sort_std: 0.0742
    global_rank: 545
    paper_rank: 545
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
    value: 0.2667
    std: 0.1242
    paper_value: 0.2667
    paper_std: 0.1242
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
    source_ref: All-in-one [22]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification using DGI pretraining; Geom-GCN 10 fixed
      splits
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.1341
    at_pub_std: null
    at_pub_source_arxiv: '2508.11328'
    at_pub_source_title: 'Aligning the Spectrum: Hybrid Graph Pre-training and Prompt
      Tuning across Homophily and Heterophily'
    at_pub_source_date_iso: '2025-08-15'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.1326
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2667
    true_std: 0.1242
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2667
    sort_std: 0.1242
    global_rank: 551
    paper_rank: 551
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Aligning the Spectrum: Hybrid Graph Pre-training and
      Prompt Tuning across Homophily and Heterophily'
    comparison_source_arxiv: '2508.11328'
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
- &id007
  dataset: Squirrel
  rows:
  - model: LMGC
    model_key: ibg-nn
    model_plain: LMGC
    value: 0.7763
    std: 0.0179
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_display: Apr 2025
    date_iso: '2025-04-25'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7763
    sort_std: 0.0179
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LMGC
    model_key: trans.conv+cna
    model_plain: LMGC
    value: 0.7747
    std: 0.0128
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7747
    sort_std: 0.0128
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LMGC
    model_key: dhgnn
    model_plain: LMGC
    value: 0.7684
    std: 0.0161
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22362'
    title: Directed Homophily-Aware Graph Neural Network
    date: May 28, 2025
    date_display: May 2025
    date_iso: '2025-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7684
    sort_std: 0.0161
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UniPrompt
    model_key: uniprompt
    model_plain: UniPrompt
    value: 0.242
    std: 0.0235
    paper_value: 0.242
    paper_std: 0.0235
    metric: Accuracy
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
    protocol_note: 1-shot node classification using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.242
    true_std: 0.0235
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.242
    sort_std: 0.0235
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
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 0.2285
    std: 0.0328
    paper_value: 0.2285
    paper_std: 0.0328
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2285
    true_std: 0.0328
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2285
    sort_std: 0.0328
    global_rank: 290
    paper_rank: 290
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Linear-probe
    model_key: linear-probe
    model_plain: Linear-probe
    value: 0.2282
    std: 0.041
    paper_value: 0.2282
    paper_std: 0.041
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
    protocol_note: 1-shot node classification using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2282
    true_std: 0.041
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2282
    sort_std: 0.041
    global_rank: 292
    paper_rank: 292
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Fine-tune
    model_key: fine-tune
    model_plain: Fine-tune
    value: 0.2227
    std: 0.041
    paper_value: 0.2227
    paper_std: 0.041
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
    protocol_note: 1-shot node classification using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2227
    true_std: 0.041
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2227
    sort_std: 0.041
    global_rank: 295
    paper_rank: 295
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
    value: 0.2203
    std: 0.0246
    paper_value: 0.2203
    paper_std: 0.0246
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
    protocol_note: 1-shot node classification using GRACE pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2203
    true_std: 0.0246
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2203
    sort_std: 0.0246
    global_rank: 297
    paper_rank: 297
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: edgeprompt+
    model_plain: EdgePrompt+
    value: 0.2199
    std: 0.025
    paper_value: 0.2199
    paper_std: 0.025
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
    protocol_note: 1-shot node classification using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2199
    true_std: 0.025
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2199
    sort_std: 0.025
    global_rank: 298
    paper_rank: 298
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
    value: 0.2166
    std: 0.0328
    paper_value: 0.2166
    paper_std: 0.0328
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
    protocol_note: 1-shot node classification using DGI pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2166
    true_std: 0.0328
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2166
    sort_std: 0.0328
    global_rank: 299
    paper_rank: 299
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPPT
    model_key: gppt
    model_plain: GPPT
    value: 0.2156
    std: 0.023
    paper_value: 0.2156
    paper_std: 0.023
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
    protocol_note: 1-shot node classification using GRACE pretraining
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2156
    true_std: 0.023
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2156
    sort_std: 0.023
    global_rank: 300
    paper_rank: 300
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
  dataset: Texas
  rows:
  - model: DoG
    model_key: p^2gnn
    model_plain: DoG
    value: 0.9672
    std: 0.0147
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9672
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.966
    std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: gpf-plus
    model_plain: DoG
    value: 0.9583
    std: 0.0419
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.05346'
    title: 'ProG: A Graph Prompt Learning Benchmark'
    date: Jun 8, 2024
    date_display: Jun 2024
    date_iso: '2024-06-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/sheldonresearch/ProG
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9583
    sort_std: 0.0419
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPF
    model_key: gpf
    model_plain: GPF
    value: 0.3483
    std: 0.1664
    paper_value: 0.3483
    paper_std: 0.1664
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
    protocol_note: 1-shot node classification; results averaged over 100 trials (20
      runs x 5 seeds).
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.874
    at_pub_std: 0.034
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.5257000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.874
    true_std: 0.034
    value_gap_source_arxiv: '2406.05346'
    value_gap_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    value_gap_source_is_current_paper: false
    value_gap: 0.5257000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.874
    sort_std: 0.034
    global_rank: 102
    paper_rank: 629
    rank_delta: 527
    rank_delta_abs: 527
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    comparison_source_arxiv: '2406.05346'
    is_best: false
    is_std_outlier: false
  - model: All-In-One
    model_key: all-in-one
    model_plain: All-In-One
    value: 0.3153
    std: 0.1314
    paper_value: 0.3153
    paper_std: 0.1314
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
    protocol_note: 1-shot node classification; results averaged over 100 trials (20
      runs x 5 seeds).
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.6549
    at_pub_std: 0.0706
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.3396
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6549
    true_std: 0.0706
    value_gap_source_arxiv: '2406.05346'
    value_gap_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    value_gap_source_is_current_paper: false
    value_gap: 0.3396
    has_value_note: false
    value_note: ''
    sort_value: 0.6549
    sort_std: 0.0706
    global_rank: 446
    paper_rank: 634
    rank_delta: 188
    rank_delta_abs: 188
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    comparison_source_arxiv: '2406.05346'
    is_best: false
    is_std_outlier: false
  - model: UniPrompt
    model_key: uniprompt
    model_plain: UniPrompt
    value: 0.4983
    std: 0.1785
    paper_value: 0.4983
    paper_std: 0.1785
    metric: Accuracy
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
    protocol_note: 1-shot node classification; results averaged over 100 trials (20
      runs x 5 seeds).
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4983
    true_std: 0.1785
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4983
    sort_std: 0.1785
    global_rank: 600
    paper_rank: 600
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Linear-probe
    model_key: linear-probe
    model_plain: Linear-probe
    value: 0.3832
    std: 0.1361
    paper_value: 0.3832
    paper_std: 0.1361
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
    protocol_note: 1-shot node classification; results averaged over 100 trials (20
      runs x 5 seeds).
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3832
    true_std: 0.1361
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3832
    sort_std: 0.1361
    global_rank: 623
    paper_rank: 623
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Fine-tune
    model_key: fine-tune
    model_plain: Fine-tune
    value: 0.375
    std: 0.1357
    paper_value: 0.375
    paper_std: 0.1357
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
    protocol_note: 1-shot node classification; results averaged over 100 trials (20
      runs x 5 seeds).
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.375
    true_std: 0.1357
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.375
    sort_std: 0.1357
    global_rank: 626
    paper_rank: 626
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPPT
    model_key: gppt
    model_plain: GPPT
    value: 0.3516
    std: 0.1512
    paper_value: 0.3516
    paper_std: 0.1512
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
    protocol_note: 1-shot node classification; results averaged over 100 trials (20
      runs x 5 seeds).
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.3181
    at_pub_std: 0.1533
    at_pub_source_arxiv: '2406.05346'
    at_pub_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    at_pub_source_date_iso: '2024-06-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.03350000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3516
    true_std: 0.1512
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3516
    sort_std: 0.1512
    global_rank: 628
    paper_rank: 628
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: edgeprompt+
    model_plain: EdgePrompt+
    value: 0.3502
    std: 0.1661
    paper_value: 0.3502
    paper_std: 0.1661
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
    protocol_note: 1-shot node classification; results averaged over 100 trials (20
      runs x 5 seeds).
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3502
    true_std: 0.1661
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3502
    sort_std: 0.1661
    global_rank: 629
    paper_rank: 629
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
    value: 0.3019
    std: 0.1363
    paper_value: 0.3019
    paper_std: 0.1363
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1-shot node classification; results averaged over 100 trials (20
      runs x 5 seeds).
    date: Sep 26, 2025
    date_display: Sep 2025
    date_iso: '2025-09-26'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-26'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3019
    true_std: 0.1363
    value_gap_source_arxiv: '2509.22416'
    value_gap_source_title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained
      Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3019
    sort_std: 0.1363
    global_rank: 635
    paper_rank: 635
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
- benchmark: Heterophilic Graphs
  datasets:
  - *id003
  - *id004
  - *id005
  - *id006
  - *id007
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: CiteSeer
      dataset_slug: citeseer
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
    - dataset: Actor
      dataset_slug: actor
    - dataset: Chameleon
      dataset_slug: chameleon
    - dataset: Squirrel
      dataset_slug: squirrel
single_proposed_model: UniPrompt
---

