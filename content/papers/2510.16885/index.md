---
title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization across Graph
  Tasks and Domains'
arxiv_id: '2510.16885'
source_url: ''
authors:
- name: Duo Wang
  orcid: null
  s2_author_id: '2317032149'
  s2_url: null
- name: Y. Zuo
  orcid: null
  s2_author_id: '1805243'
  s2_url: null
- name: Guangyue Lu
  orcid: null
  s2_author_id: '2377550350'
  s2_url: null
- name: Junjie Wu
  orcid: null
  s2_author_id: '2237788936'
  s2_url: null
published_date: Oct 19, 2025
published_date_iso: '2025-10-19'
published_venue: NeurIPS 2025
published_conference: NeurIPS 2025
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: 'Generalizing to unseen graph tasks without task-specific supervision is
  challenging: conventional graph neural networks are typically tied to a fixed label
  space, while large language models (LLMs) struggle to capture graph structure. We
  introduce UniGTE, an instruction-tuned encoder–decoder framework that unifies structural
  and semantic reasoning. The encoder augments a pretrained autoregressive LLM with
  learnable alignment tokens and a structure-aware graph–text attention mechanism,
  enabling it to attend jointly to a tokenized graph and a natural-language task prompt
  while remaining permutation-invariant to node order. This yields compact, task-aware
  graph representations. Conditioned solely on these representations, a frozen LLM
  decoder predicts and reconstructs: it outputs the task answer and simultaneously
  paraphrases the input graph in natural language. The reconstruction objective regularizes
  the encoder to preserve structural cues. UniGTE is instruction-tuned on five datasets
  spanning node-, edge-, and graph-level tasks across diverse domains, yet requires
  no fine-tuning at inference. It achieves new state-of-the-art zero-shot results
  on node classification, link prediction, graph classification and graph regression
  under cross-task and cross-domain settings, demonstrating that tight integration
  of graph structure with LLM semantics enables robust, transferable graph reasoning.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- UniGTE
mrr: 0.0025
adjusted_mrr: 0.0025
mrr_dataset_count: 4
benchmark_categories:
- Classic
- MoleculeNet
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
  total: 12
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 3
  total: 9
task_categories:
- graph_classification
- graph_regression
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id002
  dataset: Amazon-Computers
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9461
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9461
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9412
    std: 0.0008
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9412
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9398
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9398
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9351
    std: 0.0006
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 8
    sort_value: 0.9351
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaGA
    model_key: llaga
    model_plain: LLaGA
    value: 0.579
    std: null
    paper_value: 0.579
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
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Supervised results under SFT setting
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.8775
    at_pub_std: null
    at_pub_source_arxiv: '2406.10727'
    at_pub_source_title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks
      and New Insights'
    at_pub_source_date_iso: '2024-06-15'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-15'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.2985
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8775
    true_std: null
    value_gap_source_arxiv: '2406.10727'
    value_gap_source_title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks
      and New Insights'
    value_gap_source_is_current_paper: false
    value_gap: 0.2985
    has_value_note: false
    value_note: ''
    sort_value: 0.8775
    sort_std: null
    global_rank: 288
    paper_rank: 588
    rank_delta: 300
    rank_delta_abs: 300
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks
      and New Insights'
    comparison_source_arxiv: '2406.10727'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8463
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.11907'
    title: 'GraphFM: A generalist graph transformer that learns transferable representations
      across diverse domains'
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/nerdslab/GraphFM
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 394
    sort_value: 0.8463
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniGTE
    model_key: unigte
    model_plain: UniGTE
    value: 0.589
    std: null
    paper_value: 0.589
    paper_std: null
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
    protocol_note: Supervised results under SFT setting
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.589
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.589
    sort_std: null
    global_rank: 586
    paper_rank: 586
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TEA-GLM
    model_key: tea-glm
    model_plain: TEA-GLM
    value: 0.549
    std: null
    paper_value: 0.549
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
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Supervised results under SFT setting
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.578
    at_pub_std: 0.002
    at_pub_source_arxiv: '2408.14512'
    at_pub_source_title: 'LLMs as Zero-shot Graph Learners: Alignment of GNN Representations
      with LLM Token Embeddings'
    at_pub_source_date_iso: '2024-08-25'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2026-05-08'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.028999999999999915
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.578
    true_std: 0.002
    value_gap_source_arxiv: '2605.07357'
    value_gap_source_title: 'GraphReAct: Reasoning and Acting for Multi-step Graph
      Inference'
    value_gap_source_is_current_paper: false
    value_gap: 0.028999999999999915
    has_value_note: false
    value_note: ''
    sort_value: 0.578
    sort_std: 0.002
    global_rank: 589
    paper_rank: 592
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LLMs as Zero-shot Graph Learners: Alignment of GNN Representations
      with LLM Token Embeddings'
    comparison_source_arxiv: '2408.14512'
    is_best: false
    is_std_outlier: false
  - model: GOFA
    model_key: gofa
    model_plain: GOFA
    value: 0.514
    std: null
    paper_value: 0.514
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Supervised results under SFT setting
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.514
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.514
    sort_std: null
    global_rank: 594
    paper_rank: 594
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
  dataset: Amazon-Photo
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.9766
    std: 0.005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9766
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GeoMancer
    model_key: geomancer
    model_plain: GeoMancer
    value: 0.9705
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
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9705
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9703
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9643
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 13
    sort_value: 0.9643
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9128
    std: 0.0063
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_display: Jun 2023
    date_iso: '2023-06-04'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: https://github.com/GISec-Team/NCGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 434
    sort_value: 0.9128
    sort_std: 0.0063
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaGA
    model_key: llaga
    model_plain: LLaGA
    value: 0.249
    std: null
    paper_value: 0.249
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: In-domain zero-shot node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.8534
    at_pub_std: null
    at_pub_source_arxiv: '2503.03313'
    at_pub_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    at_pub_source_date_iso: '2025-03-05'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-03-05'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.6044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8534
    true_std: null
    value_gap_source_arxiv: '2503.03313'
    value_gap_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.6044
    has_value_note: false
    value_note: ''
    sort_value: 0.8534
    sort_std: null
    global_rank: 567
    paper_rank: 678
    rank_delta: 111
    rank_delta_abs: 111
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    comparison_source_arxiv: '2503.03313'
    is_best: false
    is_std_outlier: false
  - model: OFA
    model_key: ofa
    model_plain: OFA
    value: 0.317
    std: null
    paper_value: 0.317
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: In-domain zero-shot node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.8446
    at_pub_std: null
    at_pub_source_arxiv: '2503.03313'
    at_pub_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    at_pub_source_date_iso: '2025-03-05'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-03-05'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.5276000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8446
    true_std: null
    value_gap_source_arxiv: '2503.03313'
    value_gap_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.5276000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8446
    sort_std: null
    global_rank: 574
    paper_rank: 673
    rank_delta: 99
    rank_delta_abs: 99
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    comparison_source_arxiv: '2503.03313'
    is_best: false
    is_std_outlier: false
  - model: UniGTE
    model_key: unigte
    model_plain: UniGTE
    value: 0.565
    std: null
    paper_value: 0.565
    paper_std: null
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
    protocol_note: In-domain zero-shot node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.565
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.565
    sort_std: null
    global_rank: 637
    paper_rank: 637
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TEA-GLM
    model_key: tea-glm
    model_plain: TEA-GLM
    value: 0.418
    std: null
    paper_value: 0.418
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: In-domain zero-shot node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-08'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.497
    true_std: 0.027
    value_gap_source_arxiv: '2605.07357'
    value_gap_source_title: 'GraphReAct: Reasoning and Acting for Multi-step Graph
      Inference'
    value_gap_source_is_current_paper: false
    value_gap: 0.07900000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.497
    sort_std: 0.027
    global_rank: 646
    paper_rank: 655
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOFA
    model_key: gofa
    model_plain: GOFA
    value: 0.447
    std: null
    paper_value: 0.447
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: In-domain zero-shot node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.447
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.447
    sort_std: null
    global_rank: 653
    paper_rank: 653
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Vicuna-7B
    model_key: vicuna-7b
    model_plain: Vicuna-7B
    value: 0.384
    std: null
    paper_value: 0.384
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: In-domain zero-shot node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.384
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.384
    sort_std: null
    global_rank: 663
    paper_rank: 663
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
- &id004
  dataset: BACE
  rows:
  - model: ProtoMol
    model_key: protomol
    model_plain: ProtoMol
    value: 0.914
    std: 0.003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.16824'
    title: 'ProtoMol: Enhancing Molecular Property Prediction via Prototype-Guided
      Multimodal Learning'
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    venue: Briefings Bioinform.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.914
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MMSG
    model_key: mmsg
    model_plain: MMSG
    value: 0.908
    std: 0.005
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.16824'
    title: 'ProtoMol: Enhancing Molecular Property Prediction via Prototype-Guided
      Multimodal Learning'
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    venue: Briefings Bioinform.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.908
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.907
    std: 0.0
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.907
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8646
    std: 0.0081
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.15589'
    title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
      Graph Information Bottleneck
    date: Dec 20, 2024
    date_display: Dec 2024
    date_iso: '2024-12-20'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/NSLab-CUK/S-CGIB
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 41
    sort_value: 0.8646
    sort_std: 0.0081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OFA
    model_key: ofa
    model_plain: OFA
    value: 0.483
    std: null
    paper_value: 0.483
    paper_std: null
    metric: ROC-AUC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: in-domain zero-shot results
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.7788
    at_pub_std: 0.0108
    at_pub_source_arxiv: '2412.16441'
    at_pub_source_title: 'Towards Graph Foundation Models: Learning Generalities Across
      Graphs via Task-Trees'
    at_pub_source_date_iso: '2024-12-21'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.29580000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7788
    true_std: 0.0108
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.29580000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.7788
    sort_std: 0.0108
    global_rank: 216
    paper_rank: 325
    rank_delta: 109
    rank_delta_abs: 109
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    comparison_source_arxiv: '2412.16441'
    is_best: false
    is_std_outlier: false
  - model: UniGTE
    model_key: unigte
    model_plain: UniGTE
    value: 0.534
    std: null
    paper_value: 0.534
    paper_std: null
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: in-domain zero-shot results
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.534
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.534
    sort_std: null
    global_rank: 314
    paper_rank: 314
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOFA
    model_key: gofa
    model_plain: GOFA
    value: 0.5
    std: null
    paper_value: 0.5
    paper_std: null
    metric: ROC-AUC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: in-domain zero-shot results
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5
    sort_std: null
    global_rank: 322
    paper_rank: 322
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Vicuna-7B
    model_key: vicuna-7b
    model_plain: Vicuna-7B
    value: 0.492
    std: null
    paper_value: 0.492
    paper_std: null
    metric: ROC-AUC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: in-domain zero-shot results
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.492
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.492
    sort_std: null
    global_rank: 325
    paper_rank: 325
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TEA-GLM
    model_key: tea-glm
    model_plain: TEA-GLM
    value: 0.467
    std: null
    paper_value: 0.467
    paper_std: null
    metric: ROC-AUC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: in-domain zero-shot results
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.467
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.467
    sort_std: null
    global_rank: 326
    paper_rank: 326
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: ESOL
  rows:
  - model: UniGTE
    model_key: unigte
    model_plain: UniGTE
    value: 2.54
    std: null
    paper_value: 2.54
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Zero-shot performance on graph regression
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.54
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.54
    sort_std: null
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
  - model: GOFA
    model_key: gofa
    model_plain: GOFA
    value: 4.93
    std: null
    paper_value: 4.93
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Zero-shot performance on graph regression
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 4.93
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 4.93
    sort_std: null
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
  - model: Vicuna-7B
    model_key: vicuna-7b
    model_plain: Vicuna-7B
    value: 6.58
    std: null
    paper_value: 6.58
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Zero-shot performance on graph regression
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.58
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.58
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
  - model: TEA-GLM
    model_key: tea-glm
    model_plain: TEA-GLM
    value: 14.9
    std: null
    paper_value: 14.9
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Zero-shot performance on graph regression
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 14.9
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 14.9
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
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id006
  dataset: FreeSolv
  rows:
  - model: DCT
    model_key: dct
    model_plain: DCT
    value: 1.339
    std: 0.075
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 1
    sort_value: 1.339
    sort_std: 0.075
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UniAug
    model_key: uniaug
    model_plain: UniAug
    value: 1.448
    std: 0.049
    metric: MAE
    higher_is_better: false
    is_baseline: true
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
    sort_value: 1.448
    sort_std: 0.049
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FLAG
    model_key: flag
    model_plain: FLAG
    value: 1.565
    std: 0.098
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 3
    sort_value: 1.565
    sort_std: 0.098
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 1.613
    std: 0.155
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 4
    sort_value: 1.613
    sort_std: 0.155
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniGTE
    model_key: unigte
    model_plain: UniGTE
    value: 9.18
    std: null
    paper_value: 9.18
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Zero-shot performance on cross-task graph regression.
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 9.18
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 9.18
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
  - model: TEA-GLM
    model_key: tea-glm
    model_plain: TEA-GLM
    value: 13.35
    std: null
    paper_value: 13.35
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Zero-shot performance on cross-task graph regression.
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 13.35
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 13.35
    sort_std: null
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOFA
    model_key: gofa
    model_plain: GOFA
    value: 14.98
    std: null
    paper_value: 14.98
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Zero-shot performance on cross-task graph regression.
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 14.98
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 14.98
    sort_std: null
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Vicuna-7B
    model_key: vicuna-7b
    model_plain: Vicuna-7B
    value: 64.11
    std: null
    paper_value: 64.11
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Zero-shot performance on cross-task graph regression.
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 64.11
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 64.11
    sort_std: null
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id003
  dataset: WikiCS
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9302
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9302
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RSE + RGCN (70b)
    model_key: rse + rgcn (70b)
    model_plain: RSE + RGCN (70b)
    value: 0.8852
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 2
    sort_value: 0.8852
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LEMP+T
    model_key: lemp+t
    model_plain: LEMP+T
    value: 0.8825
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8825
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8771
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 9
    sort_value: 0.8771
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaGA
    model_key: llaga
    model_plain: LLaGA
    value: 0.601
    std: null
    paper_value: 0.601
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot performance on node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.8074
    at_pub_std: null
    at_pub_source_arxiv: '2503.03313'
    at_pub_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    at_pub_source_date_iso: '2025-03-05'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-03-05'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.20640000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8074
    true_std: null
    value_gap_source_arxiv: '2503.03313'
    value_gap_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.20640000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8074
    sort_std: null
    global_rank: 85
    paper_rank: 337
    rank_delta: 252
    rank_delta_abs: 252
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    comparison_source_arxiv: '2503.03313'
    is_best: false
    is_std_outlier: false
  - model: GOFA
    model_key: gofa
    model_plain: GOFA
    value: 0.613
    std: null
    paper_value: 0.613
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot performance on node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.7996
    at_pub_std: null
    at_pub_source_arxiv: '2407.09709'
    at_pub_source_title: 'GOFA: A Generative One-For-All Model for Joint Graph Language
      Modeling'
    at_pub_source_date_iso: '2024-07-12'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-07-12'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.1866
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7996
    true_std: null
    value_gap_source_arxiv: '2407.09709'
    value_gap_source_title: 'GOFA: A Generative One-For-All Model for Joint Graph
      Language Modeling'
    value_gap_source_is_current_paper: false
    value_gap: 0.1866
    has_value_note: false
    value_note: ''
    sort_value: 0.7996
    sort_std: null
    global_rank: 105
    paper_rank: 335
    rank_delta: 230
    rank_delta_abs: 230
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GOFA: A Generative One-For-All Model for Joint Graph
      Language Modeling'
    comparison_source_arxiv: '2407.09709'
    is_best: false
    is_std_outlier: false
  - model: OFA
    model_key: ofa
    model_plain: OFA
    value: 0.361
    std: null
    paper_value: 0.361
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot performance on node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.7855
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2505.12684'
    at_pub_source_title: Towards Effective Federated Graph Foundation Model via Mitigating
      Knowledge Entanglement
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.4245
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7855
    true_std: 0.0037
    value_gap_source_arxiv: '2505.12684'
    value_gap_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    value_gap_source_is_current_paper: false
    value_gap: 0.4245
    has_value_note: false
    value_note: ''
    sort_value: 0.7855
    sort_std: 0.0037
    global_rank: 163
    paper_rank: 348
    rank_delta: 185
    rank_delta_abs: 185
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    comparison_source_arxiv: '2505.12684'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7469
    std: 0.0085
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.11561'
    title: 'View Space: Learning Representation across Arbitrary Graphs'
    date: Dec 12, 2025
    date_display: Dec 2025
    date_iso: '2025-12-12'
    venue: Accepted to ICML 2026
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 246
    sort_value: 0.7469
    sort_std: 0.0085
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniGTE
    model_key: unigte
    model_plain: UniGTE
    value: 0.68
    std: null
    paper_value: 0.68
    paper_std: null
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
    protocol_note: Zero-shot performance on node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.68
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.68
    sort_std: null
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
  - model: TEA-GLM
    model_key: tea-glm
    model_plain: TEA-GLM
    value: 0.449
    std: null
    paper_value: 0.449
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot performance on node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.449
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.449
    sort_std: null
    global_rank: 347
    paper_rank: 347
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Vicuna-7B
    model_key: vicuna-7b
    model_plain: Vicuna-7B
    value: 0.29
    std: null
    paper_value: 0.29
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot performance on node classification
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.29
    true_std: null
    value_gap_source_arxiv: '2510.16885'
    value_gap_source_title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization
      across Graph Tasks and Domains'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.29
    sort_std: null
    global_rank: 352
    paper_rank: 352
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
  - *id003
- benchmark: MoleculeNet
  datasets:
  - *id004
  - *id005
  - *id006
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
    - dataset: WikiCS
      dataset_slug: wikics
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: BACE
      dataset_slug: bace
    - dataset: ESOL
      dataset_slug: esol
    - dataset: FreeSolv
      dataset_slug: freesolv
single_proposed_model: UniGTE
main_figure: /figures/2510.16885/main_figure.jpegoptim.jpg
---

