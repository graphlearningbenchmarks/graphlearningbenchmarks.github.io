---
title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
arxiv_id: '2603.00599'
source_url: ''
authors:
- name: Li Sun
  orcid: null
  s2_author_id: '2276663165'
  s2_url: null
- name: Ming Zhang
  orcid: null
  s2_author_id: '2287880406'
  s2_url: null
- name: Wenxin Jin
  orcid: null
  s2_author_id: '2421639385'
  s2_url: null
- name: Zhongtian Sun
  orcid: null
  s2_author_id: '1446912194'
  s2_url: null
- name: Zhenhao Huang
  orcid: null
  s2_author_id: '2277686441'
  s2_url: null
- name: Hao Peng
  orcid: null
  s2_author_id: '2314564206'
  s2_url: null
- name: Sen Su
  orcid: null
  s2_author_id: '2269441658'
  s2_url: null
- name: Philip Yu
  orcid: null
  s2_author_id: '2277626629'
  s2_url: null
published_date: Feb 28, 2026
published_date_iso: '2026-02-28'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Hypergraphs are the natural description of higher-order interactions among
  objects, widely applied in social network analysis, cross-modal retrieval, etc.
  Hypergraph Neural Networks (HGNNs) have become the dominant solution for learning
  on hypergraphs. Traditional HGNNs are extended from message passing graph neural
  networks, following the homophily assumption, and thus struggle with the prevalent
  heterophilic hypergraphs that call for long-range dependence modeling. Existing
  solutions enlarge the message flow through the hypergraph bottleneck, mitigating
  the oversquashing issue and capturing long-range dependence. However, they often
  accelerate the loss of representation distinguishability in the repeated aggregations,
  leading to oversmoothing. This dilemma motivates an interesting question: Can we
  develop a unified mechanism that is agnostic to both homophilic and heterophilic
  hypergraphs? In this paper, we achieve the best of both worlds through the lens
  of Riemannian geometry, which provides the potential to adjust the message passing
  behavior in different regions. The key insight lies in the connection between oversquashing
  and hypergraph bottleneck within the framework of Riemannian manifold heat flow.
  Building on this, we propose the novel idea of locally adapting the bottlenecks
  of different subhypergraphs. The core innovation of the proposed mechanism is the
  design of an adaptive local (heat) exchanger. Specifically, it captures the rich
  long-range dependencies via the Robin condition, and preserves the representation
  distinguishability via source terms, thereby enabling heterophily-agnostic message
  passing with theoretical guarantees. Based on this theoretical foundation, we present
  a novel Heat-Exchanger with Adaptive Locality for Hypergraph Neural Network (HealHGNN),
  designed as a node-hyperedge bidirectional systems with linear complexity in the
  number of nodes and hyperedges. Extensive experiments on both homophilic and heterophilic
  cases show that HealHGNN achieves the state-of-the-art performance.'
codebase_url: https://github.com/Mingzhang21/HealHGNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- HealHGNN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Hypergraph Benchmarks
benchmark_coverage:
- benchmark: Hypergraph Benchmarks
  benchmark_slug: hypergraph-benchmarks
  evaluated: 5
  total: 10
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
  dataset: Congress
  rows:
  - model: HealHGNN
    model_key: healhgnn
    model_plain: HealHGNN
    value: 0.9345
    std: 0.0079
    paper_value: 0.9345
    paper_std: 0.0079
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9345
    true_std: 0.0079
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9345
    sort_std: 0.0079
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
  - model: ED-HNN
    model_key: ed-hnn
    model_plain: ED-HNN
    value: 0.9328
    std: 0.0059
    paper_value: 0.9328
    paper_std: 0.0059
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
    source_ref: ICLR22-edhnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9328
    true_std: 0.0059
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9328
    sort_std: 0.0059
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
  - model: KHGNN
    model_key: khgnn
    model_plain: KHGNN
    value: 0.9255
    std: 0.0103
    paper_value: 0.9255
    paper_std: 0.0103
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
    source_ref: AAAI25-KHGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9255
    true_std: 0.0103
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9255
    sort_std: 0.0103
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Deep-HGNN
    model_key: deep-hgnn
    model_plain: Deep-HGNN
    value: 0.9247
    std: 0.0106
    paper_value: 0.9247
    paper_std: 0.0106
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
    source_ref: arxiv22-deephgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9247
    true_std: 0.0106
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9247
    sort_std: 0.0106
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UniGCNII
    model_key: unigcnii
    model_plain: UniGCNII
    value: 0.9243
    std: 0.0071
    paper_value: 0.9243
    paper_std: 0.0071
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
    source_ref: arxiv21-hgnn-uniGCNII
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9243
    true_std: 0.0071
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9243
    sort_std: 0.0071
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AllSetTransformer
    model_key: allsettransformer
    model_plain: AllSetTransformer
    value: 0.9216
    std: 0.0105
    paper_value: 0.9216
    paper_std: 0.0105
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: iclr22-alldeepsets-allsettrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9216
    true_std: 0.0105
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9216
    sort_std: 0.0105
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SheafHyperGNN
    model_key: sheafhypergnn
    model_plain: SheafHyperGNN
    value: 0.9181
    std: 0.016
    paper_value: 0.9181
    paper_std: 0.016
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
    source_ref: NIPS23-sheafhypergnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9181
    true_std: 0.016
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9181
    sort_std: 0.016
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AllDeepSets
    model_key: alldeepsets
    model_plain: AllDeepSets
    value: 0.918
    std: 0.0153
    paper_value: 0.918
    paper_std: 0.0153
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
    source_ref: iclr22-alldeepsets-allsettrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.918
    true_std: 0.0153
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.918
    sort_std: 0.0153
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HGNN
    model_key: hgnn
    model_plain: HGNN
    value: 0.9126
    std: 0.0115
    paper_value: 0.9126
    paper_std: 0.0115
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
    source_ref: AAAI19-hgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9126
    true_std: 0.0115
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9126
    sort_std: 0.0115
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
  - model: HNHN
    model_key: hnhn
    model_plain: HNHN
    value: 0.9089
    std: 0.0031
    paper_value: 0.9089
    paper_std: 0.0031
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
    source_ref: arxiv20-hnhn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9089
    true_std: 0.0031
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9089
    sort_std: 0.0031
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
  - model: HCHA
    model_key: hcha
    model_plain: HCHA
    value: 0.9043
    std: 0.012
    paper_value: 0.9043
    paper_std: 0.012
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
    source_ref: PR21-hcha
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9043
    true_std: 0.012
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9043
    sort_std: 0.012
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
  - model: PhenomNN
    model_key: phenomnn
    model_plain: PhenomNN
    value: 0.8824
    std: 0.0147
    paper_value: 0.8824
    paper_std: 0.0147
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
    source_ref: ICML24-PhenomNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8824
    true_std: 0.0147
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8824
    sort_std: 0.0147
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HyperGCN
    model_key: hypergcn
    model_plain: HyperGCN
    value: 0.8743
    std: 0.0146
    paper_value: 0.8743
    paper_std: 0.0146
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
    source_ref: nips19-hypergcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8743
    true_std: 0.0146
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8743
    sort_std: 0.0146
    global_rank: 13
    paper_rank: 13
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
  dataset: DBLP-CA
  rows:
  - model: HealHGNN
    model_key: healhgnn
    model_plain: HealHGNN
    value: 0.9198
    std: 0.0031
    paper_value: 0.9198
    paper_std: 0.0031
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9198
    true_std: 0.0031
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9198
    sort_std: 0.0031
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
  - model: AllSetTransformer
    model_key: allsettransformer
    model_plain: AllSetTransformer
    value: 0.9153
    std: 0.0023
    paper_value: 0.9153
    paper_std: 0.0023
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: iclr22-alldeepsets-allsettrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9198
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2406.06642'
    at_pub_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    at_pub_source_date_iso: '2024-06-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0044999999999999485
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9198
    true_std: 0.0018
    value_gap_source_arxiv: '2406.06642'
    value_gap_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0044999999999999485
    has_value_note: false
    value_note: ''
    sort_value: 0.9198
    sort_std: 0.0018
    global_rank: 2
    paper_rank: 7
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'TopoBench: A Framework for Benchmarking Topological
      Deep Learning'
    comparison_source_arxiv: '2406.06642'
    is_best: true
    is_std_outlier: false
  - model: ED-HNN
    model_key: ed-hnn
    model_plain: ED-HNN
    value: 0.919
    std: 0.0019
    paper_value: 0.919
    paper_std: 0.0019
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
    source_ref: ICLR22-edhnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.919
    true_std: 0.0019
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.919
    sort_std: 0.0019
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PhenomNN
    model_key: phenomnn
    model_plain: PhenomNN
    value: 0.9186
    std: 0.0022
    paper_value: 0.9186
    paper_std: 0.0022
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
    source_ref: ICML24-PhenomNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9186
    true_std: 0.0022
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9186
    sort_std: 0.0022
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Deep-HGNN
    model_key: deep-hgnn
    model_plain: Deep-HGNN
    value: 0.9176
    std: 0.0028
    paper_value: 0.9176
    paper_std: 0.0028
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
    source_ref: arxiv22-deephgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9176
    true_std: 0.0028
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9176
    sort_std: 0.0028
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UniGCNII
    model_key: unigcnii
    model_plain: UniGCNII
    value: 0.9169
    std: 0.0019
    paper_value: 0.9169
    paper_std: 0.0019
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
    source_ref: arxiv21-hgnn-uniGCNII
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9169
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9169
    true_std: 0.0019
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9169
    sort_std: 0.0019
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SheafHyperGNN
    model_key: sheafhypergnn
    model_plain: SheafHyperGNN
    value: 0.9159
    std: 0.0024
    paper_value: 0.9159
    paper_std: 0.0024
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
    source_ref: NIPS23-sheafhypergnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9159
    true_std: 0.0024
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9159
    sort_std: 0.0024
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AllDeepSets
    model_key: alldeepsets
    model_plain: AllDeepSets
    value: 0.9127
    std: 0.0027
    paper_value: 0.9127
    paper_std: 0.0027
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
    source_ref: iclr22-alldeepsets-allsettrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9127
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9127
    true_std: 0.0027
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9127
    sort_std: 0.0027
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
  - model: KHGNN
    model_key: khgnn
    model_plain: KHGNN
    value: 0.9121
    std: 0.0037
    paper_value: 0.9121
    paper_std: 0.0037
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
    source_ref: AAAI25-KHGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9121
    true_std: 0.0037
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9121
    sort_std: 0.0037
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
  - model: HGNN
    model_key: hgnn
    model_plain: HGNN
    value: 0.9103
    std: 0.002
    paper_value: 0.9103
    paper_std: 0.002
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
    source_ref: AAAI19-hgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9103
    at_pub_std: 0.002
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9103
    true_std: 0.002
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9103
    sort_std: 0.002
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
  - model: HCHA
    model_key: hcha
    model_plain: HCHA
    value: 0.9092
    std: 0.0022
    paper_value: 0.9092
    paper_std: 0.0022
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
    source_ref: PR21-hcha
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9092
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9092
    true_std: 0.0022
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9092
    sort_std: 0.0022
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HyperGCN
    model_key: hypergcn
    model_plain: HyperGCN
    value: 0.8998
    std: 0.0043
    paper_value: 0.8998
    paper_std: 0.0043
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
    source_ref: nips19-hypergcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8938
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8998
    true_std: 0.0043
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8998
    sort_std: 0.0043
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HNHN
    model_key: hnhn
    model_plain: HNHN
    value: 0.8678
    std: 0.0029
    paper_value: 0.8678
    paper_std: 0.0029
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
    source_ref: arxiv20-hnhn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8678
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8678
    true_std: 0.0029
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8678
    sort_std: 0.0029
    global_rank: 19
    paper_rank: 19
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
    value: 0.8483
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_display: Jun 2021
    date_iso: '2021-06-24'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jianhao2016/AllSet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 20
    sort_value: 0.8483
    sort_std: 0.0022
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
- &id001
  dataset: House
  rows:
  - model: HealHGNN
    model_key: healhgnn
    model_plain: HealHGNN
    value: 0.7718
    std: 0.0235
    paper_value: 0.7718
    paper_std: 0.0235
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7718
    true_std: 0.0235
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7718
    sort_std: 0.0235
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
  - model: Deep-HGNN
    model_key: deep-hgnn
    model_plain: Deep-HGNN
    value: 0.7526
    std: 0.0176
    paper_value: 0.7526
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
    source_ref: arxiv22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7526
    true_std: 0.0176
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7526
    sort_std: 0.0176
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
  - model: mechanism (shared)
    model_key: mechanism (shared)
    model_plain: mechanism (shared)
    value: 0.747
    std: 0.0756
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_display: Aug 2023
    date_iso: '2023-08-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.747
    sort_std: 0.0756
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: KHGNN
    model_key: khgnn
    model_plain: KHGNN
    value: 0.7431
    std: 0.0287
    paper_value: 0.7431
    paper_std: 0.0287
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
    source_ref: AAAI25
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7431
    true_std: 0.0287
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7431
    sort_std: 0.0287
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SheafHyperGNN
    model_key: sheafhypergnn
    model_plain: SheafHyperGNN
    value: 0.7384
    std: 0.023
    paper_value: 0.7384
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
    source_ref: NIPS23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7384
    true_std: 0.023
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7384
    sort_std: 0.023
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FrameHGNN
    model_key: framehgnn
    model_plain: FrameHGNN
    value: 0.7282
    std: 0.0222
    paper_value: 0.7282
    paper_std: 0.0222
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
    source_ref: AAAI25
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7282
    true_std: 0.0222
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7282
    sort_std: 0.0222
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ED-HNN
    model_key: ed-hnn
    model_plain: ED-HNN
    value: 0.7245
    std: 0.0228
    paper_value: 0.7245
    paper_std: 0.0228
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
    source_ref: ICLR22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7245
    true_std: 0.0228
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7245
    sort_std: 0.0228
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
  - model: PhenomNN
    model_key: phenomnn
    model_plain: PhenomNN
    value: 0.7071
    std: 0.0235
    paper_value: 0.7071
    paper_std: 0.0235
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
    source_ref: ICML24
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7071
    true_std: 0.0235
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7071
    sort_std: 0.0235
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
  - model: AllSetTransformer
    model_key: allsettransformer
    model_plain: AllSetTransformer
    value: 0.6983
    std: 0.0522
    paper_value: 0.6983
    paper_std: 0.0522
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: iclr22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6933
    at_pub_std: 0.022
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6983
    true_std: 0.0522
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6983
    sort_std: 0.0522
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6793
    std: 0.0233
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_display: Jun 2021
    date_iso: '2021-06-24'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jianhao2016/AllSet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 12
    sort_value: 0.6793
    sort_std: 0.0233
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AllDeepSets
    model_key: alldeepsets
    model_plain: AllDeepSets
    value: 0.6782
    std: 0.024
    paper_value: 0.6782
    paper_std: 0.024
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
    source_ref: iclr22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6782
    at_pub_std: 0.024
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6782
    true_std: 0.024
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6782
    sort_std: 0.024
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HNHN
    model_key: hnhn
    model_plain: HNHN
    value: 0.678
    std: 0.0259
    paper_value: 0.678
    paper_std: 0.0259
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
    source_ref: arxiv20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.678
    at_pub_std: 0.0259
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.678
    true_std: 0.0259
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.678
    sort_std: 0.0259
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniGCNII
    model_key: unigcnii
    model_plain: UniGCNII
    value: 0.6725
    std: 0.0257
    paper_value: 0.6725
    paper_std: 0.0257
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
    source_ref: arxiv21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6725
    at_pub_std: 0.0257
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6725
    true_std: 0.0257
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6725
    sort_std: 0.0257
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGNN
    model_key: hgnn
    model_plain: HGNN
    value: 0.6139
    std: 0.0296
    paper_value: 0.6139
    paper_std: 0.0296
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
    source_ref: AAAI19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6139
    at_pub_std: 0.0296
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6139
    true_std: 0.0296
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6139
    sort_std: 0.0296
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HCHA
    model_key: hcha
    model_plain: HCHA
    value: 0.6136
    std: 0.0253
    paper_value: 0.6136
    paper_std: 0.0253
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
    source_ref: PR21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6136
    at_pub_std: 0.0253
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6136
    true_std: 0.0253
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6136
    sort_std: 0.0253
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HyperGCN
    model_key: hypergcn
    model_plain: HyperGCN
    value: 0.6013
    std: 0.0176
    paper_value: 0.6013
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
    source_ref: nips19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4831
    at_pub_std: 0.0293
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.11819999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6013
    true_std: 0.0176
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6013
    sort_std: 0.0176
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Hypergraph Benchmarks
    comparison_source_arxiv: '2106.13264'
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
- &id005
  dataset: Senate
  rows:
  - model: HealHGNN
    model_key: healhgnn
    model_plain: HealHGNN
    value: 0.7606
    std: 0.0413
    paper_value: 0.7606
    paper_std: 0.0413
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7606
    true_std: 0.0413
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7606
    sort_std: 0.0413
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
  - model: KHGNN
    model_key: khgnn
    model_plain: KHGNN
    value: 0.7123
    std: 0.0394
    paper_value: 0.7123
    paper_std: 0.0394
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
    source_ref: AAAI25-KHGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7123
    true_std: 0.0394
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7123
    sort_std: 0.0394
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
  - model: AllSetTransformer
    model_key: allsettransformer
    model_plain: AllSetTransformer
    value: 0.6933
    std: 0.022
    paper_value: 0.6933
    paper_std: 0.022
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: iclr22-alldeepsets-allsettrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6933
    true_std: 0.022
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6933
    sort_std: 0.022
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
  - model: SheafHyperGNN
    model_key: sheafhypergnn
    model_plain: SheafHyperGNN
    value: 0.6873
    std: 0.0468
    paper_value: 0.6873
    paper_std: 0.0468
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
    source_ref: NIPS23-sheafhypergnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6873
    true_std: 0.0468
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6873
    sort_std: 0.0468
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Deep-HGNN
    model_key: deep-hgnn
    model_plain: Deep-HGNN
    value: 0.6839
    std: 0.0479
    paper_value: 0.6839
    paper_std: 0.0479
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
    source_ref: arxiv22-deephgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6839
    true_std: 0.0479
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6839
    sort_std: 0.0479
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PhenomNN
    model_key: phenomnn
    model_plain: PhenomNN
    value: 0.677
    std: 0.0524
    paper_value: 0.677
    paper_std: 0.0524
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
    source_ref: ICML24-PhenomNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.677
    true_std: 0.0524
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.677
    sort_std: 0.0524
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FrameHGNN
    model_key: framehgnn
    model_plain: FrameHGNN
    value: 0.6761
    std: 0.0527
    paper_value: 0.6761
    paper_std: 0.0527
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
    source_ref: AAAI25-FrameHGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6761
    true_std: 0.0527
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6761
    sort_std: 0.0527
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ED-HNN
    model_key: ed-hnn
    model_plain: ED-HNN
    value: 0.6479
    std: 0.0514
    paper_value: 0.6479
    paper_std: 0.0514
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
    source_ref: ICLR22-edhnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6479
    true_std: 0.0514
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6479
    sort_std: 0.0514
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
  - model: HNHN
    model_key: hnhn
    model_plain: HNHN
    value: 0.5093
    std: 0.0633
    paper_value: 0.5093
    paper_std: 0.0633
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
    source_ref: arxiv20-hnhn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5093
    true_std: 0.0633
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5093
    sort_std: 0.0633
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
  - model: HyperGCN
    model_key: hypergcn
    model_plain: HyperGCN
    value: 0.5013
    std: 0.0321
    paper_value: 0.5013
    paper_std: 0.0321
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
    source_ref: nips19-hypergcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5013
    true_std: 0.0321
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5013
    sort_std: 0.0321
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
  - model: UniGCNII
    model_key: unigcnii
    model_plain: UniGCNII
    value: 0.493
    std: 0.0425
    paper_value: 0.493
    paper_std: 0.0425
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
    source_ref: arxiv21-hgnn-uniGCNII
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.493
    true_std: 0.0425
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.493
    sort_std: 0.0425
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
  - model: HCHA
    model_key: hcha
    model_plain: HCHA
    value: 0.4862
    std: 0.0441
    paper_value: 0.4862
    paper_std: 0.0441
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
    source_ref: PR21-hcha
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4862
    true_std: 0.0441
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4862
    sort_std: 0.0441
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGNN
    model_key: hgnn
    model_plain: HGNN
    value: 0.4859
    std: 0.0452
    paper_value: 0.4859
    paper_std: 0.0452
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
    source_ref: AAAI19-hgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4859
    true_std: 0.0452
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4859
    sort_std: 0.0452
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AllDeepSets
    model_key: alldeepsets
    model_plain: AllDeepSets
    value: 0.4817
    std: 0.0567
    paper_value: 0.4817
    paper_std: 0.0567
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
    source_ref: iclr22-alldeepsets-allsettrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4817
    true_std: 0.0567
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4817
    sort_std: 0.0567
    global_rank: 14
    paper_rank: 14
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
  dataset: Walmart
  rows:
  - model: HealHGNN
    model_key: healhgnn
    model_plain: HealHGNN
    value: 0.6822
    std: 0.0056
    paper_value: 0.6822
    paper_std: 0.0056
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6822
    true_std: 0.0056
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6822
    sort_std: 0.0056
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
  - model: ED-HNN
    model_key: ed-hnn
    model_plain: ED-HNN
    value: 0.6679
    std: 0.0041
    paper_value: 0.6679
    paper_std: 0.0041
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
    source_ref: ICLR22-edhnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6679
    true_std: 0.0041
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6679
    sort_std: 0.0041
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
  - model: AllSetTransformer
    model_key: allsettransformer
    model_plain: AllSetTransformer
    value: 0.6546
    std: 0.0025
    paper_value: 0.6546
    paper_std: 0.0025
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: iclr22-alldeepsets-allsettrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6546
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6546
    true_std: 0.0025
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6546
    sort_std: 0.0025
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
  - model: KHGNN
    model_key: khgnn
    model_plain: KHGNN
    value: 0.6517
    std: 0.0079
    paper_value: 0.6517
    paper_std: 0.0079
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
    source_ref: AAAI25-KHGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6517
    true_std: 0.0079
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6517
    sort_std: 0.0079
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
  - model: AllDeepSets
    model_key: alldeepsets
    model_plain: AllDeepSets
    value: 0.6455
    std: 0.0033
    paper_value: 0.6455
    paper_std: 0.0033
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
    source_ref: iclr22-alldeepsets-allsettrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6455
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6455
    true_std: 0.0033
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6455
    sort_std: 0.0033
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
  - model: PhenomNN
    model_key: phenomnn
    model_plain: PhenomNN
    value: 0.6343
    std: 0.0043
    paper_value: 0.6343
    paper_std: 0.0043
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
    source_ref: ICML24-PhenomNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6343
    true_std: 0.0043
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6343
    sort_std: 0.0043
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
  - model: HCHA
    model_key: hcha
    model_plain: HCHA
    value: 0.6235
    std: 0.0026
    paper_value: 0.6235
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
    source_ref: PR21-hcha
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6245
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-06-24'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6245
    true_std: 0.0026
    value_gap_source_arxiv: '2106.13264'
    value_gap_source_title: Hypergraph Benchmarks
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.6245
    sort_std: 0.0026
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGNN
    model_key: hgnn
    model_plain: HGNN
    value: 0.62
    std: 0.0024
    paper_value: 0.62
    paper_std: 0.0024
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
    source_ref: AAAI19-hgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.62
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.62
    true_std: 0.0024
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.62
    sort_std: 0.0024
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
  - model: Deep-HGNN
    model_key: deep-hgnn
    model_plain: Deep-HGNN
    value: 0.5864
    std: 0.0074
    paper_value: 0.5864
    paper_std: 0.0074
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
    source_ref: arxiv22-deephgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5864
    true_std: 0.0074
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5864
    sort_std: 0.0074
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
  - model: UniGCNII
    model_key: unigcnii
    model_plain: UniGCNII
    value: 0.5445
    std: 0.0037
    paper_value: 0.5445
    paper_std: 0.0037
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
    source_ref: arxiv21-hgnn-uniGCNII
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5445
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5445
    true_std: 0.0037
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5445
    sort_std: 0.0037
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
  - model: HNHN
    model_key: hnhn
    model_plain: HNHN
    value: 0.5118
    std: 0.0035
    paper_value: 0.5118
    paper_std: 0.0035
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
    source_ref: arxiv20-hnhn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4718
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5118
    true_std: 0.0035
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5118
    sort_std: 0.0035
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Hypergraph Benchmarks
    comparison_source_arxiv: '2106.13264'
    is_best: false
    is_std_outlier: false
  - model: HyperGCN
    model_key: hypergcn
    model_plain: HyperGCN
    value: 0.4874
    std: 0.0281
    paper_value: 0.4874
    paper_std: 0.0281
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
    source_ref: nips19-hypergcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4474
    at_pub_std: 0.0281
    at_pub_source_arxiv: '2106.13264'
    at_pub_source_title: Hypergraph Benchmarks
    at_pub_source_date_iso: '2021-06-24'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.03999999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4874
    true_std: 0.0281
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4874
    sort_std: 0.0281
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4551
    std: 0.0024
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_display: Jun 2021
    date_iso: '2021-06-24'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jianhao2016/AllSet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 16
    sort_value: 0.4551
    sort_std: 0.0024
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
- benchmark: Hypergraph Benchmarks
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Hypergraph Benchmarks
    benchmark_slug: hypergraph-benchmarks
    datasets:
    - dataset: House
      dataset_slug: house
    - dataset: DBLP-CA
      dataset_slug: dblp-ca
    - dataset: Walmart
      dataset_slug: walmart
    - dataset: Congress
      dataset_slug: congress
    - dataset: Senate
      dataset_slug: senate
single_proposed_model: HealHGNN
main_figure: /figures/2603.00599/main_figure.jpegoptim.jpg
---

