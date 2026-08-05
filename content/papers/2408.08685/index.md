---
title: Can Large Language Models Improve the Adversarial Robustness of Graph Neural
  Networks?
arxiv_id: '2408.08685'
source_url: ''
authors:
- name: Zhongjian Zhang
  orcid: null
  s2_author_id: '2284728816'
  s2_url: null
- name: Xiao Wang
  orcid: null
  s2_author_id: '2118449003'
  s2_url: null
- name: Huichi Zhou
  orcid: null
  s2_author_id: '2283313383'
  s2_url: null
- name: Yue Yu
  orcid: null
  s2_author_id: '2257366050'
  s2_url: null
- name: Mengmei Zhang
  orcid: null
  s2_author_id: '16003017'
  s2_url: null
- name: Cheng Yang
  orcid: null
  s2_author_id: '2257052319'
  s2_url: null
- name: Chuan Shi
  orcid: null
  s2_author_id: '2293890214'
  s2_url: null
published_date: Aug 16, 2024
published_date_iso: '2024-08-16'
published_venue: KDD 2024
published_conference: KDD 2024
published_conference_short: KDD
published_conference_slug: kdd
abstract: 'Graph neural networks (GNNs) are vulnerable to adversarial attacks, especially
  for topology perturbations, and many methods that improve the robustness of GNNs
  have received considerable attention. Recently, we have witnessed the significant
  success of large language models (LLMs), leading many to explore the great potential
  of LLMs on GNNs. However, they mainly focus on improving the performance of GNNs
  by utilizing LLMs to enhance the node features. Therefore, we ask: Will the robustness
  of GNNs also be enhanced with the powerful understanding and inference capabilities
  of LLMs? By presenting the empirical results, we find that despite that LLMs can
  improve the robustness of GNNs, there is still an average decrease of 23.1\'
codebase_url: https://github.com/zhongjian-zhang/LLM4RGNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN LLM4RGNN
- GAT LLM4RGNN
- RGCN LLM4RGNN
- SimP-GCN LLM4RGNN
mrr: 0.0047
adjusted_mrr: 0.0016
mrr_dataset_count: 1
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
  - model: GCN vanilla
    model_key: gcn vanilla
    model_plain: GCN vanilla
    value: 0.7986
    std: 0.0015
    paper_value: 0.7986
    paper_std: 0.0015
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Non-targeted attack (Mettack) with 0% perturbation rate
    date: Aug 16, 2024
    date_display: Aug 2024
    date_iso: '2024-08-16'
    published_venue: KDD 2024
    published_conference: KDD 2024
    at_pub_value: 0.787
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2110.14855'
    at_pub_source_title: 'CAP: Co-Adversarial Perturbation on Weights and Features
      for Improving Generalization of Graph Neural Networks'
    at_pub_source_date_iso: '2021-10-28'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-08-16'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.011599999999999944
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7986
    true_std: 0.0015
    value_gap_source_arxiv: '2408.08685'
    value_gap_source_title: Can Large Language Models Improve the Adversarial Robustness
      of Graph Neural Networks?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7986
    sort_std: 0.0015
    global_rank: 173
    paper_rank: 173
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'CAP: Co-Adversarial Perturbation on Weights and Features
      for Improving Generalization of Graph Neural Networks'
    comparison_source_arxiv: '2110.14855'
    is_best: false
    is_std_outlier: false
  - model: GAT Vanilla
    model_key: gat vanilla
    model_plain: GAT Vanilla
    value: 0.7875
    std: 0.0026
    paper_value: 0.7875
    paper_std: 0.0026
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Non-targeted attack (Mettack) with 0% perturbation rate
    date: Aug 16, 2024
    date_display: Aug 2024
    date_iso: '2024-08-16'
    published_venue: KDD 2024
    published_conference: KDD 2024
    at_pub_value: 0.7945
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2110.14855'
    at_pub_source_title: 'CAP: Co-Adversarial Perturbation on Weights and Features
      for Improving Generalization of Graph Neural Networks'
    at_pub_source_date_iso: '2021-10-28'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.007000000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7945
    true_std: 0.0059
    value_gap_source_arxiv: '2110.14855'
    value_gap_source_title: 'CAP: Co-Adversarial Perturbation on Weights and Features
      for Improving Generalization of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.007000000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.7945
    sort_std: 0.0059
    global_rank: 191
    paper_rank: 227
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN LLM4RGNN
    model_key: gcn llm4rgnn
    model_plain: GCN LLM4RGNN
    value: 0.7904
    std: 0.0042
    paper_value: 0.7904
    paper_std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Non-targeted attack (Mettack) with 0% perturbation rate
    date: Aug 16, 2024
    date_display: Aug 2024
    date_iso: '2024-08-16'
    published_venue: KDD 2024
    published_conference: KDD 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-16'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7904
    true_std: 0.0042
    value_gap_source_arxiv: '2408.08685'
    value_gap_source_title: Can Large Language Models Improve the Adversarial Robustness
      of Graph Neural Networks?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7904
    sort_std: 0.0042
    global_rank: 215
    paper_rank: 215
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN Vanilla
    model_key: rgcn vanilla
    model_plain: RGCN Vanilla
    value: 0.7845
    std: 0.0025
    paper_value: 0.7845
    paper_std: 0.0025
    metric: Accuracy
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Non-targeted attack (Mettack) with 0% perturbation rate
    date: Aug 16, 2024
    date_display: Aug 2024
    date_iso: '2024-08-16'
    published_venue: KDD 2024
    published_conference: KDD 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-16'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7845
    true_std: 0.0025
    value_gap_source_arxiv: '2408.08685'
    value_gap_source_title: Can Large Language Models Improve the Adversarial Robustness
      of Graph Neural Networks?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7845
    sort_std: 0.0025
    global_rank: 243
    paper_rank: 243
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN LLM4RGNN
    model_key: rgcn llm4rgnn
    model_plain: RGCN LLM4RGNN
    value: 0.7783
    std: 0.0048
    paper_value: 0.7783
    paper_std: 0.0048
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Non-targeted attack (Mettack) with 0% perturbation rate
    date: Aug 16, 2024
    date_display: Aug 2024
    date_iso: '2024-08-16'
    published_venue: KDD 2024
    published_conference: KDD 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-16'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7783
    true_std: 0.0048
    value_gap_source_arxiv: '2408.08685'
    value_gap_source_title: Can Large Language Models Improve the Adversarial Robustness
      of Graph Neural Networks?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7783
    sort_std: 0.0048
    global_rank: 252
    paper_rank: 252
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT LLM4RGNN
    model_key: gat llm4rgnn
    model_plain: GAT LLM4RGNN
    value: 0.7776
    std: 0.0062
    paper_value: 0.7776
    paper_std: 0.0062
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Non-targeted attack (Mettack) with 0% perturbation rate
    date: Aug 16, 2024
    date_display: Aug 2024
    date_iso: '2024-08-16'
    published_venue: KDD 2024
    published_conference: KDD 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-16'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7776
    true_std: 0.0062
    value_gap_source_arxiv: '2408.08685'
    value_gap_source_title: Can Large Language Models Improve the Adversarial Robustness
      of Graph Neural Networks?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7776
    sort_std: 0.0062
    global_rank: 254
    paper_rank: 254
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimP-GCN Vanilla
    model_key: simp-gcn vanilla
    model_plain: SimP-GCN Vanilla
    value: 0.7587
    std: 0.0036
    paper_value: 0.7587
    paper_std: 0.0036
    metric: Accuracy
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Non-targeted attack (Mettack) with 0% perturbation rate
    date: Aug 16, 2024
    date_display: Aug 2024
    date_iso: '2024-08-16'
    published_venue: KDD 2024
    published_conference: KDD 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-16'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7587
    true_std: 0.0036
    value_gap_source_arxiv: '2408.08685'
    value_gap_source_title: Can Large Language Models Improve the Adversarial Robustness
      of Graph Neural Networks?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7587
    sort_std: 0.0036
    global_rank: 280
    paper_rank: 280
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimP-GCN LLM4RGNN
    model_key: simp-gcn llm4rgnn
    model_plain: SimP-GCN LLM4RGNN
    value: 0.7584
    std: 0.0029
    paper_value: 0.7584
    paper_std: 0.0029
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Non-targeted attack (Mettack) with 0% perturbation rate
    date: Aug 16, 2024
    date_display: Aug 2024
    date_iso: '2024-08-16'
    published_venue: KDD 2024
    published_conference: KDD 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-16'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7584
    true_std: 0.0029
    value_gap_source_arxiv: '2408.08685'
    value_gap_source_title: Can Large Language Models Improve the Adversarial Robustness
      of Graph Neural Networks?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7584
    sort_std: 0.0029
    global_rank: 281
    paper_rank: 281
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
    global_rank: 394
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
main_figure: /figures/2408.08685/main_figure.jpegoptim.jpg
---

