---
title: Improving Subgraph Extraction for Graph Invariant Learning via Graph Sinkhorn
  Attention
arxiv_id: '2402.07191'
source_url: ''
authors:
- name: Junchi Yan
  orcid: null
  s2_author_id: '2283878108'
  s2_url: null
- name: Fangyu Ding
  orcid: null
  s2_author_id: '2283850232'
  s2_url: null
- name: Jiawei Sun
  orcid: null
  s2_author_id: '2319176592'
  s2_url: null
- name: Zhaoping Hu
  orcid: null
  s2_author_id: '2283878004'
  s2_url: null
- name: Yunyi Zhou
  orcid: null
  s2_author_id: '2311822276'
  s2_url: null
- name: Lei Zhu
  orcid: null
  s2_author_id: '2341674848'
  s2_url: null
published_date: Feb 11, 2024
published_date_iso: '2024-02-11'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph invariant learning (GIL) seeks invariant relations between graphs
  and labels under distribution shifts. Recent works try to extract an invariant subgraph
  to improve out-of-distribution (OOD) generalization, yet existing approaches either
  lack explicit control over compactness or rely on hard top-$k$ selection that shrinks
  the solution space and is only partially differentiable. In this paper, we provide
  an in-depth analysis of the drawbacks of some existing works and propose a few general
  principles for invariant subgraph extraction: 1) separability, as encouraged by
  our sparsity-driven mechanism, to filter out the irrelevant common features; 2)
  softness, for a broader solution space; and 3) differentiability, for a soundly
  end-to-end optimization pipeline. Specifically, building on optimal transport, we
  propose Graph Sinkhorn Attention (GSINA), a fully differentiable, cardinality-constrained
  attention mechanism that assigns sparse-yet-soft edge weights via Sinkhorn iterations
  and induces node attention. GSINA provides explicit controls for separability and
  softness, and uses a Gumbel reparameterization to stabilize training. It convergence
  behavior is also theoretically studied. Extensive empirical experimental results
  on both synthetic and real-world datasets validate its superiority.'
codebase_url: https://github.com/dingfangyu/GSINA
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GIN+GSINA
- PNA+GSINA
- GSINA
mrr: 0.0166
adjusted_mrr: 0.0166
mrr_dataset_count: 3
benchmark_categories:
- TU Dortmund
- OGB
- MoleculeNet
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 3
  total: 9
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id004
  dataset: ClinTox
  rows:
  - model: EdgePrompt+
    model_key: se(3)-i mpph
    model_plain: EdgePrompt+
    value: 0.993
    std: 0.004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_display: Dec 2023
    date_iso: '2023-12-12'
    venue: NeurIPS 2023 AI for Science Workshop
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: integrating SE(3)-invariance into Vietoris-Rips persistent
      homology
    is_global_top: true
    global_rank: 1
    sort_value: 0.993
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: ka-gcn
    model_plain: EdgePrompt+
    value: 0.992
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
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.992
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: ka-gat
    model_plain: EdgePrompt+
    value: 0.991
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
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.991
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GSINA
    model_key: gsina
    model_plain: GSINA
    value: 0.9008
    std: 0.0206
    paper_value: 0.9008
    paper_std: 0.0206
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
    variant_inference_reason: 'dataset: fuzzy match to clintox (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGBG-Mol datasets follow standard OOD generalization evaluation
      as per OGB/miao2022interpretable.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9008
    true_std: 0.0206
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9008
    sort_std: 0.0206
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
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.878
    std: 0.0236
    paper_value: 0.878
    paper_std: 0.0236
    metric: ROC-AUC
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
    source_ref: miao2022interpretable
    variant_inference_reason: 'dataset: fuzzy match to clintox (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGBG-Mol datasets follow standard OOD generalization evaluation
      as per OGB/miao2022interpretable.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.875
    at_pub_std: 0.027
    at_pub_source_arxiv: '2305.15745'
    at_pub_source_title: Robust Ante-hoc Graph Explainer using Bilevel Optimization
    at_pub_source_date_iso: '2023-05-25'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.878
    true_std: 0.0236
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.878
    sort_std: 0.0236
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.8672
    std: 0.0233
    paper_value: 0.8672
    paper_std: 0.0233
    metric: ROC-AUC
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
    source_ref: corso2020principal
    variant_inference_reason: 'dataset: fuzzy match to clintox (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGBG-Mol datasets follow standard OOD generalization evaluation
      as per OGB/miao2022interpretable.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.867
    at_pub_std: 0.011
    at_pub_source_arxiv: '2309.10131'
    at_pub_source_title: Deep Prompt Tuning for Graph Transformers
    at_pub_source_date_iso: '2023-09-18'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8672
    true_std: 0.0233
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8672
    sort_std: 0.0233
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
- &id001
  dataset: NCI1
  rows:
  - model: Oracle (IID)
    model_key: oracle (iid)
    model_plain: Oracle (IID)
    value: 0.32
    std: 0.05
    paper_value: 0.32
    paper_std: 0.05
    metric: MCC
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
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.32
    true_std: 0.05
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.32
    sort_std: 0.05
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
  - model: IGM
    model_key: igm
    model_plain: IGM
    value: 0.28
    std: 0.04
    paper_value: 0.28
    paper_std: 0.04
    metric: MCC
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
    source_ref: jia2024graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.28
    true_std: 0.04
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.28
    sort_std: 0.04
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
  - model: GSINA
    model_key: gsina
    model_plain: GSINA
    value: 0.28
    std: 0.07
    paper_value: 0.28
    paper_std: 0.07
    metric: MCC
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
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.28
    true_std: 0.07
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.28
    sort_std: 0.07
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
  - model: CIGAv2
    model_key: cigav2
    model_plain: CIGAv2
    value: 0.27
    std: 0.07
    paper_value: 0.27
    paper_std: 0.07
    metric: MCC
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
    source_ref: chen2022learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.27
    true_std: 0.07
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.27
    sort_std: 0.07
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
  - model: SUGAR
    model_key: sugar
    model_plain: SUGAR
    value: 0.27
    std: 0.06
    paper_value: 0.27
    paper_std: 0.06
    metric: MCC
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
    source_ref: liu2025subgraph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.27
    true_std: 0.06
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.27
    sort_std: 0.06
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
  - model: CIGAv1
    model_key: cigav1
    model_plain: CIGAv1
    value: 0.22
    std: 0.07
    paper_value: 0.22
    paper_std: 0.07
    metric: MCC
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
    source_ref: chen2022learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.22
    true_std: 0.07
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.22
    sort_std: 0.07
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
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.21
    std: 0.06
    paper_value: 0.21
    paper_std: 0.06
    metric: MCC
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
    source_ref: wu2022discovering
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.21
    true_std: 0.06
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.21
    sort_std: 0.06
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
  - model: IRM
    model_key: irm
    model_plain: IRM
    value: 0.17
    std: 0.02
    paper_value: 0.17
    paper_std: 0.02
    metric: MCC
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
    source_ref: arjovsky2019invariant
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.17
    true_std: 0.02
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.17
    sort_std: 0.02
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
  - model: CNC
    model_key: cnc
    model_plain: CNC
    value: 0.16
    std: 0.04
    paper_value: 0.16
    paper_std: 0.04
    metric: MCC
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
    source_ref: Zhang_Sohoni_Zhang_Finn_R
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.16
    true_std: 0.04
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.16
    sort_std: 0.04
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
  - model: ASAP
    model_key: asap
    model_plain: ASAP
    value: 0.16
    std: 0.1
    paper_value: 0.16
    paper_std: 0.1
    metric: MCC
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
    source_ref: ranjan2019asap
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.16
    true_std: 0.1
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.16
    sort_std: 0.1
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
  - model: ERM
    model_key: erm
    model_plain: ERM
    value: 0.15
    std: 0.05
    paper_value: 0.15
    paper_std: 0.05
    metric: MCC
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
    source_ref: Vapnik 1991
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.15
    true_std: 0.05
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.15
    sort_std: 0.05
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
  - model: V-REx
    model_key: v-rex
    model_plain: V-REx
    value: 0.15
    std: 0.04
    paper_value: 0.15
    paper_std: 0.04
    metric: MCC
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
    source_ref: krueger2021out
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.15
    true_std: 0.04
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.15
    sort_std: 0.04
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
  - model: EIIL
    model_key: eiil
    model_plain: EIIL
    value: 0.14
    std: 0.03
    paper_value: 0.14
    paper_std: 0.03
    metric: MCC
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
    source_ref: Creager_Jacobsen_Zemel_2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.14
    true_std: 0.03
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.14
    sort_std: 0.03
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
  - model: GIB
    model_key: gib
    model_plain: GIB
    value: 0.13
    std: 0.1
    paper_value: 0.13
    paper_std: 0.1
    metric: MCC
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
    source_ref: yu2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.13
    true_std: 0.1
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.13
    sort_std: 0.1
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
  - model: IB-IRM
    model_key: ib-irm
    model_plain: IB-IRM
    value: 0.12
    std: 0.04
    paper_value: 0.12
    paper_std: 0.04
    metric: MCC
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
    source_ref: ahuja2021invariance
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: MCC is the standard metric for TU datasets as per text; task is
      graph-level OOD generalization.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.12
    true_std: 0.04
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.12
    sort_std: 0.04
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
  rank_metric: MCC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - MCC
  metric: MCC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id005
  dataset: SIDER
  rows:
  - model: DGI
    model_key: ka-gat
    model_plain: DGI
    value: 0.847
    std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.847
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DGI
    model_key: ka-gcn
    model_plain: DGI
    value: 0.842
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.842
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: graphkan
    model_plain: DGI
    value: 0.837
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.837
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.5758
    std: 0.0123
    paper_value: 0.5758
    paper_std: 0.0123
    metric: ROC-AUC
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
    source_ref: miao2022interpretable
    variant_inference_reason: 'dataset: fuzzy match to sider (score=77)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGBG-Mol datasets follow standard OOD generalization evaluation
      for OGBG.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.5919
    true_std: 0.0103
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.016100000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.5919
    sort_std: 0.0103
    global_rank: 202
    paper_rank: 218
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSINA
    model_key: gsina
    model_plain: GSINA
    value: 0.5861
    std: 0.0109
    paper_value: 0.5861
    paper_std: 0.0109
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
    variant_inference_reason: 'dataset: fuzzy match to sider (score=77)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGBG-Mol datasets follow standard OOD generalization evaluation
      for OGBG.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5861
    true_std: 0.0109
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5861
    sort_std: 0.0109
    global_rank: 207
    paper_rank: 207
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.5651
    std: 0.019
    paper_value: 0.5651
    paper_std: 0.019
    metric: ROC-AUC
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
    source_ref: corso2020principal
    variant_inference_reason: 'dataset: fuzzy match to sider (score=77)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGBG-Mol datasets follow standard OOD generalization evaluation
      for OGBG.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.583
    at_pub_std: 0.012
    at_pub_source_arxiv: '2309.10131'
    at_pub_source_title: Deep Prompt Tuning for Graph Transformers
    at_pub_source_date_iso: '2023-09-18'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-09-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.017899999999999916
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.583
    true_std: 0.012
    value_gap_source_arxiv: '2309.10131'
    value_gap_source_title: Deep Prompt Tuning for Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.017899999999999916
    has_value_note: false
    value_note: ''
    sort_value: 0.583
    sort_std: 0.012
    global_rank: 211
    paper_rank: 229
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
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
- &id003
  dataset: Tox21
  rows:
  - model: HOD-GNN
    model_key: himp
    model_plain: HOD-GNN
    value: 0.874
    std: 0.005
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.874
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HOD-GNN
    model_key: gine w/ vn
    model_plain: HOD-GNN
    value: 0.872
    std: 0.003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.872
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HOD-GNN
    model_key: naivegine+ k=3 w/ vn
    model_plain: HOD-GNN
    value: 0.87
    std: 0.004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.87
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.7508
    std: 0.0064
    paper_value: 0.7508
    paper_std: 0.0064
    metric: ROC-AUC
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
    source_ref: corso2020principal
    variant_inference_reason: 'dataset: fuzzy match to tox21 (score=77)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGBG-Moltox21 task using ROC-AUC as specified in the text for OGBG
      datasets.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.793
    at_pub_std: 0.015
    at_pub_source_arxiv: '2309.10131'
    at_pub_source_title: Deep Prompt Tuning for Graph Transformers
    at_pub_source_date_iso: '2023-09-18'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-09-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.042200000000000015
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.793
    true_std: 0.015
    value_gap_source_arxiv: '2309.10131'
    value_gap_source_title: Deep Prompt Tuning for Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.042200000000000015
    has_value_note: false
    value_note: ''
    sort_value: 0.793
    sort_std: 0.015
    global_rank: 86
    paper_rank: 224
    rank_delta: 138
    rank_delta_abs: 138
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Deep Prompt Tuning for Graph Transformers
    comparison_source_arxiv: '2309.10131'
    is_best: false
    is_std_outlier: false
  - model: GSINA
    model_key: gsina
    model_plain: GSINA
    value: 0.7547
    std: 0.0055
    paper_value: 0.7547
    paper_std: 0.0055
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
    variant_inference_reason: 'dataset: fuzzy match to tox21 (score=77)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGBG-Moltox21 task using ROC-AUC as specified in the text for OGBG
      datasets.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7547
    true_std: 0.0055
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7547
    sort_std: 0.0055
    global_rank: 204
    paper_rank: 204
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.7496
    std: 0.0066
    paper_value: 0.7496
    paper_std: 0.0066
    metric: ROC-AUC
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
    source_ref: miao2022interpretable
    variant_inference_reason: 'dataset: fuzzy match to tox21 (score=77)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGBG-Moltox21 task using ROC-AUC as specified in the text for OGBG
      datasets.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.729
    at_pub_std: 0.009
    at_pub_source_arxiv: '2305.15745'
    at_pub_source_title: Robust Ante-hoc Graph Explainer using Bilevel Optimization
    at_pub_source_date_iso: '2023-05-25'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.020600000000000063
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7496
    true_std: 0.0066
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7496
    sort_std: 0.0066
    global_rank: 229
    paper_rank: 229
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Robust Ante-hoc Graph Explainer using Bilevel Optimization
    comparison_source_arxiv: '2305.15745'
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
- &id002
  dataset: ogbg-molhiv
  rows:
  - model: SigGate-GT
    model_key: multi-rf fusion with multi-gnn blending
    model_plain: SigGate-GT
    value: 0.8476
    std: 0.0002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: mixed
    feature_source_evidence: Mixing pharmacophoric (FCFP) and structural (ECFP) fingerprints...
      GNNs contributing only 12%
    is_global_top: true
    global_rank: 1
    sort_value: 0.8476
    sort_std: 0.0002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: hyperfusion
    model_plain: SigGate-GT
    value: 0.8475
    std: 0.0003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8475
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: pas+fps
    model_plain: SigGate-GT
    value: 0.842
    std: 0.0015
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.842
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA+GSINA
    model_key: pna+gsina
    model_plain: PNA+GSINA
    value: 0.8055
    std: 0.0097
    paper_value: 0.8055
    paper_std: 0.0097
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
    protocol_note: OOD generalization on GSAT benchmark using scaffold split.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8055
    true_std: 0.0097
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8055
    sort_std: 0.0097
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
  - model: PNA+GSAT
    model_key: pna+gsat
    model_plain: PNA+GSAT
    value: 0.8024
    std: 0.0073
    paper_value: 0.8024
    paper_std: 0.0073
    metric: ROC-AUC
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
    source_ref: miao2022interpretable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization on GSAT benchmark using scaffold split.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8024
    true_std: 0.0073
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8024
    sort_std: 0.0073
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
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.7891
    std: 0.0104
    paper_value: 0.7891
    paper_std: 0.0104
    metric: ROC-AUC
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
    source_ref: corso2020principal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization on GSAT benchmark using scaffold split.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7905
    at_pub_std: 0.0132
    at_pub_source_arxiv: '2103.16584'
    at_pub_source_title: Parameterized Hypercomplex Graph Neural Networks for Graph
      Classification
    at_pub_source_date_iso: '2021-03-30'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.0013999999999999568
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7905
    true_std: 0.0132
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.0013999999999999568
    has_value_note: false
    value_note: ''
    sort_value: 0.7905
    sort_std: 0.0132
    global_rank: 68
    paper_rank: 71
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+GSINA
    model_key: gin+gsina
    model_plain: GIN+GSINA
    value: 0.7799
    std: 0.0097
    paper_value: 0.7799
    paper_std: 0.0097
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
    protocol_note: OOD generalization on GSAT benchmark using scaffold split.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7799
    true_std: 0.0097
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7799
    sort_std: 0.0097
    global_rank: 112
    paper_rank: 112
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.7669
    std: 0.0125
    paper_value: 0.7669
    paper_std: 0.0125
    metric: ROC-AUC
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
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization on GSAT benchmark using scaffold split.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.778
    at_pub_std: 0.0182
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.011099999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.778
    true_std: 0.0182
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.011099999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.0182
    global_rank: 120
    paper_rank: 182
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.7634
    std: 0.0101
    paper_value: 0.7634
    paper_std: 0.0101
    metric: ROC-AUC
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
    source_ref: wu2022discovering
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization on GSAT benchmark using scaffold split.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7705
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2201.12872'
    at_pub_source_title: Discovering Invariant Rationales for Graph Neural Networks
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.007099999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7705
    true_std: 0.0057
    value_gap_source_arxiv: '2201.12872'
    value_gap_source_title: Discovering Invariant Rationales for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.007099999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7705
    sort_std: 0.0057
    global_rank: 164
    paper_rank: 200
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+GSAT
    model_key: gin+gsat
    model_plain: GIN+GSAT
    value: 0.7647
    std: 0.0153
    paper_value: 0.7647
    paper_std: 0.0153
    metric: ROC-AUC
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
    source_ref: miao2022interpretable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization on GSAT benchmark using scaffold split.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7647
    true_std: 0.0153
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7647
    sort_std: 0.0153
    global_rank: 197
    paper_rank: 197
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIB
    model_key: gib
    model_plain: GIB
    value: 0.7643
    std: 0.0265
    paper_value: 0.7643
    paper_std: 0.0265
    metric: ROC-AUC
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
    source_ref: yu2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization on GSAT benchmark using scaffold split.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7643
    true_std: 0.0265
    value_gap_source_arxiv: '2402.07191'
    value_gap_source_title: Improving Subgraph Extraction for Graph Invariant Learning
      via Graph Sinkhorn Attention
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7643
    sort_std: 0.0265
    global_rank: 199
    paper_rank: 199
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
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
- benchmark: OGB
  datasets:
  - *id002
- benchmark: MoleculeNet
  datasets:
  - *id003
  - *id004
  - *id005
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: NCI1
      dataset_slug: nci1
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: Tox21
      dataset_slug: tox21
    - dataset: ClinTox
      dataset_slug: clintox
    - dataset: SIDER
      dataset_slug: sider
main_figure: /figures/2402.07191/main_figure.jpegoptim.jpg
---

