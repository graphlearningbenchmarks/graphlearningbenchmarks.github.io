---
title: Learning Hierarchical Protein Representations via Complete 3D Graph Networks
arxiv_id: '2207.12600'
source_url: ''
authors:
- name: Limei Wang
  orcid: null
  s2_author_id: '2109120459'
  s2_url: null
- name: Haoran Liu
  orcid: null
  s2_author_id: '2143857491'
  s2_url: null
- name: Yi Liu
  orcid: null
  s2_author_id: '2153630672'
  s2_url: null
- name: Jerry Kurtin
  orcid: null
  s2_author_id: '2179190141'
  s2_url: null
- name: Shuiwang Ji
  orcid: null
  s2_author_id: '1743600'
  s2_url: null
published_date: Jul 26, 2022
published_date_iso: '2022-07-26'
published_venue: ICLR 2022
published_conference: ICLR 2022
published_conference_short: ICLR
published_conference_slug: iclr
abstract: We consider representation learning for proteins with 3D structures. We
  build 3D graphs based on protein structures and develop graph networks to learn
  their representations. Depending on the levels of details that we wish to capture,
  protein representations can be computed at different levels, e.g., the amino acid,
  backbone, or all-atom levels. Importantly, there exist hierarchical relations among
  different levels. In this work, we propose to develop a novel hierarchical graph
  network, known as ProNet, to capture the relations. Our ProNet is very flexible
  and can be used to compute protein representations at different levels of granularity.
  By treating each amino acid as a node in graph modeling as well as harnessing the
  inherent hierarchies, our ProNet is more effective and efficient than existing methods.
  We also show that, given a base 3D graph network that is complete, our ProNet representations
  are also complete at all levels. Experimental results show that ProNet outperforms
  recent methods on most datasets. In addition, results indicate that different downstream
  tasks may require representations at different levels. Our code is publicly available
  as part of the DIG library.
codebase_url: https://github.com/divelab/DIG
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ProNet-Amino Acid
- ProNet-Backbone
- ProNet-All-Atom
mrr: 0.0
adjusted_mrr: 0.0
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
  dataset: PPI
  rows:
  - model: ProNet-All-Atom
    model_key: pronet-all-atom
    model_plain: ProNet-All-Atom
    value: 0.871
    std: null
    paper_value: 0.871
    paper_std: null
    metric: AUROC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Results on the PPI task using AUROC metric.
    date: Jul 26, 2022
    date_display: Jul 2022
    date_iso: '2022-07-26'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.871
    true_std: null
    value_gap_source_arxiv: '2207.12600'
    value_gap_source_title: Learning Hierarchical Protein Representations via Complete
      3D Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.871
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
  - model: GVP-GNN
    model_key: gvp-gnn
    model_plain: GVP-GNN
    value: 0.866
    std: null
    paper_value: 0.866
    paper_std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: jing2021equivariant
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Results on the PPI task using AUROC metric.
    date: Jul 26, 2022
    date_display: Jul 2022
    date_iso: '2022-07-26'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.866
    true_std: null
    value_gap_source_arxiv: '2207.12600'
    value_gap_source_title: Learning Hierarchical Protein Representations via Complete
      3D Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.866
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
  - model: ProNet-Backbone
    model_key: pronet-backbone
    model_plain: ProNet-Backbone
    value: 0.858
    std: null
    paper_value: 0.858
    paper_std: null
    metric: AUROC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Results on the PPI task using AUROC metric.
    date: Jul 26, 2022
    date_display: Jul 2022
    date_iso: '2022-07-26'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.858
    true_std: null
    value_gap_source_arxiv: '2207.12600'
    value_gap_source_title: Learning Hierarchical Protein Representations via Complete
      3D Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.858
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
  - model: ProNet-Amino Acid
    model_key: pronet-amino acid
    model_plain: ProNet-Amino Acid
    value: 0.857
    std: null
    paper_value: 0.857
    paper_std: null
    metric: AUROC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Results on the PPI task using AUROC metric.
    date: Jul 26, 2022
    date_display: Jul 2022
    date_iso: '2022-07-26'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.857
    true_std: null
    value_gap_source_arxiv: '2207.12600'
    value_gap_source_title: Learning Hierarchical Protein Representations via Complete
      3D Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.857
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
  - model: Atom3D-3DCNN
    model_key: atom3d-3dcnn
    model_plain: Atom3D-3DCNN
    value: 0.844
    std: null
    paper_value: 0.844
    paper_std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: townshend2021atomd
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Results on the PPI task using AUROC metric.
    date: Jul 26, 2022
    date_display: Jul 2022
    date_iso: '2022-07-26'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.844
    true_std: null
    value_gap_source_arxiv: '2207.12600'
    value_gap_source_title: Learning Hierarchical Protein Representations via Complete
      3D Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.844
    sort_std: null
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
  - model: Atom3D-GNN
    model_key: atom3d-gnn
    model_plain: Atom3D-GNN
    value: 0.669
    std: null
    paper_value: 0.669
    paper_std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: townshend2021atomd
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Results on the PPI task using AUROC metric.
    date: Jul 26, 2022
    date_display: Jul 2022
    date_iso: '2022-07-26'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.669
    true_std: null
    value_gap_source_arxiv: '2207.12600'
    value_gap_source_title: Learning Hierarchical Protein Representations via Complete
      3D Graph Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.669
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
  rank_metric: AUROC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - AUROC
  metric: AUROC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
    - dataset: PPI
      dataset_slug: ppi
---

