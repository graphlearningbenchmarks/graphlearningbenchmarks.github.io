---
title: 'Clustering as Reasoning: A $k$-Means Interpretation of Chain-of-Thought Graph
  Learning'
arxiv_id: '2605.24867'
source_url: ''
authors:
- name: Xuanting Xie
  orcid: null
  s2_author_id: '2197705751'
  s2_url: null
- name: Zhaochen Guo
  orcid: null
  s2_author_id: '2335507545'
  s2_url: null
- name: Bingheng Li
  orcid: null
  s2_author_id: '2276175028'
  s2_url: null
- name: Xingtong Yu
  orcid: null
  s2_author_id: '2204706384'
  s2_url: null
- name: Zhifei Liao
  orcid: null
  s2_author_id: '2438713368'
  s2_url: null
- name: Zhao Kang
  orcid: null
  s2_author_id: '2275599913'
  s2_url: null
- name: Yuan Fang
  orcid: null
  s2_author_id: '2281289986'
  s2_url: null
published_date: May 24, 2026
published_date_iso: '2026-05-24'
published_venue: ICML 2026
published_conference: ICML 2026
published_conference_short: ICML
published_conference_slug: icml
abstract: Chain-of-Thought (CoT) prompting has shown promise in enhancing the reasoning
  capabilities of large language models (LLMs) on text-attributed graphs (TAGs). This
  work reframes CoT-based graph learning through the principle of clustering as reasoning,
  offering a $k$-means interpretation of how iterative reasoning operates over graph-structured
  data. We observe that existing graph CoT methods rely on disjoint architectures
  and fixed graph representations, limiting step-by-step semantic-topological interaction
  and interpretability. To overcome this limitation, we propose a unified framework
  named KCoT that integrates CoT reasoning with graph representation learning. Our
  key theoretical result reveals a formal mathematical correspondence between a Transformer
  block and the $k$-means algorithm, allowing reasoning to be interpreted as iterative
  assignment and update steps. Based on this insight, we introduce a Semantic Discriminating
  Prompt that explicitly formulates these steps as structured CoT reasoning, together
  with a structure-grounded alignment strategy to fuse topological priors with evolving
  thought-conditioned representations. Experiments on standard benchmarks demonstrate
  consistent improvements over state-of-the-art methods, validating clustering as
  a principled mechanism for CoT-based graph learning.
codebase_url: https://github.com/Uncnbb/KCoT
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: ogbn-products
  rows:
  - model: Jacobi
    model_key: jacobi
    model_plain: Jacobi
    value: 0.8968
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
    global_rank: 1
    sort_value: 0.8968
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPR
    model_key: gpr
    model_plain: GPR
    value: 0.8953
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
    global_rank: 2
    sort_value: 0.8953
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LEMP4HG
    model_key: lemp4hg
    model_plain: LEMP4HG
    value: 0.8939
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
    sort_value: 0.8939
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8933
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
    global_rank: 4
    sort_value: 0.8933
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8306
    std: null
    paper_value: 0.8306
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node Classification Accuracy on ogbn-products using Single Focus
      protocol (trained on individual task-dataset pair).
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    published_venue: ICML 2026
    published_conference: ICML 2026
    at_pub_value: 0.8829
    at_pub_std: null
    at_pub_source_arxiv: '2505.19762'
    at_pub_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    at_pub_source_date_iso: '2025-05-26'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.05230000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8829
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.05230000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8829
    sort_std: null
    global_rank: 9
    paper_rank: 78
    rank_delta: 69
    rank_delta_abs: 69
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    comparison_source_arxiv: '2505.19762'
    is_best: false
    is_std_outlier: false
  - model: SAGN
    model_key: sagn
    model_plain: SAGN
    value: 0.8258
    std: null
    paper_value: 0.8258
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node Classification Accuracy on ogbn-products using Single Focus
      protocol (trained on individual task-dataset pair).
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    published_venue: ICML 2026
    published_conference: ICML 2026
    at_pub_value: 0.8736
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2210.14709'
    at_pub_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    at_pub_source_date_iso: 2022-10
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.047800000000000065
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8736
    true_std: 0.0007
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: false
    value_gap: 0.047800000000000065
    has_value_note: false
    value_note: ''
    sort_value: 0.8736
    sort_std: 0.0007
    global_rank: 14
    paper_rank: 83
    rank_delta: 69
    rank_delta_abs: 69
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    comparison_source_arxiv: '2210.14709'
    is_best: false
    is_std_outlier: false
  - model: LLAGA-HO
    model_key: llaga-ho
    model_plain: LLAGA-HO
    value: 0.8467
    std: null
    paper_value: 0.8467
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node Classification Accuracy on ogbn-products using Single Focus
      protocol (trained on individual task-dataset pair).
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    published_venue: ICML 2026
    published_conference: ICML 2026
    at_pub_value: 0.7364
    at_pub_std: null
    at_pub_source_arxiv: '2501.15755'
    at_pub_source_title: 'GraphICL: Unlocking Graph Learning Potential in LLMs through
      Structured Prompt Design'
    at_pub_source_date_iso: '2025-01-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.11029999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8467
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8467
    sort_std: null
    global_rank: 49
    paper_rank: 49
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphICL: Unlocking Graph Learning Potential in LLMs
      through Structured Prompt Design'
    comparison_source_arxiv: '2501.15755'
    is_best: false
    is_std_outlier: false
  - model: LLAGA-ND
    model_key: llaga-nd
    model_plain: LLAGA-ND
    value: 0.846
    std: null
    paper_value: 0.846
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node Classification Accuracy on ogbn-products using Single Focus
      protocol (trained on individual task-dataset pair).
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    published_venue: ICML 2026
    published_conference: ICML 2026
    at_pub_value: 0.7362
    at_pub_std: null
    at_pub_source_arxiv: '2501.15755'
    at_pub_source_title: 'GraphICL: Unlocking Graph Learning Potential in LLMs through
      Structured Prompt Design'
    at_pub_source_date_iso: '2025-01-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.10980000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.846
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.846
    sort_std: null
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphICL: Unlocking Graph Learning Potential in LLMs
      through Structured Prompt Design'
    comparison_source_arxiv: '2501.15755'
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.8372
    std: null
    paper_value: 0.8372
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node Classification Accuracy on ogbn-products using Single Focus
      protocol (trained on individual task-dataset pair).
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    published_venue: ICML 2026
    published_conference: ICML 2026
    at_pub_value: 0.6726
    at_pub_std: 0.0071
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.16460000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8372
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8372
    sort_std: null
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    comparison_source_arxiv: '2401.15569'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8287
    std: null
    paper_value: 0.8287
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node Classification Accuracy on ogbn-products using Single Focus
      protocol (trained on individual task-dataset pair).
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    published_venue: ICML 2026
    published_conference: ICML 2026
    at_pub_value: 0.8061
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2210.07494'
    at_pub_source_title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking
      and Rethinking'
    at_pub_source_date_iso: '2022-10-14'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.022599999999999953
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8287
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8287
    sort_std: null
    global_rank: 82
    paper_rank: 82
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    comparison_source_arxiv: '2210.07494'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7547
    std: null
    paper_value: 0.7547
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node Classification Accuracy on ogbn-products using Single Focus
      protocol (trained on individual task-dataset pair).
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    published_venue: ICML 2026
    published_conference: ICML 2026
    at_pub_value: 0.822
    at_pub_std: 0.009
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.06729999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.822
    true_std: 0.009
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.06729999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.009
    global_rank: 93
    paper_rank: 268
    rank_delta: 175
    rank_delta_abs: 175
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6605
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2211.16199'
    title: Latent Graph Inference using Product Manifolds
    date: Nov 26, 2022
    date_display: Nov 2022
    date_iso: '2022-11-26'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 361
    sort_value: 0.6605
    sort_std: 0.002
    comparison_type: global_top
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
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
main_figure: /figures/2605.24867/main_figure.jpegoptim.jpg
---

