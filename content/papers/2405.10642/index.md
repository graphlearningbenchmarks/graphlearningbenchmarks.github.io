---
title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
arxiv_id: '2405.10642'
source_url: ''
authors:
- name: Chuang Liu
  orcid: null
  s2_author_id: '145760439'
  s2_url: null
- name: Zelin Yao
  orcid: null
  s2_author_id: '2298560734'
  s2_url: null
- name: Xueqi Ma
  orcid: null
  s2_author_id: '2249043738'
  s2_url: null
- name: Mukun Chen
  orcid: null
  s2_author_id: '2108227988'
  s2_url: null
- name: Luzhi Wang
  orcid: null
  s2_author_id: '2278588129'
  s2_url: null
- name: Jia Wu
  orcid: null
  s2_author_id: '2248803714'
  s2_url: null
- name: Wenbin Hu
  orcid: null
  s2_author_id: '2146226874'
  s2_url: null
published_date: May 17, 2024
published_date_iso: '2024-05-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Masked Autoencoders (GMAEs) have emerged as a notable self-supervised
  learning approach for graph-structured data. Existing GMAE models primarily focus
  on reconstructing node-level information, categorizing them as single-scale GMAEs.
  This methodology, while effective in certain contexts, tends to overlook the complex
  hierarchical structures inherent in many real-world graphs. For instance, molecular
  graphs exhibit a clear hierarchical organization in the form of the atoms-functional
  groups-molecules structure. Therefore, the inability of single-scale GMAE models
  to incorporate these hierarchical relationships often results in an inadequate capture
  of crucial high-level graph information, leading to a noticeable decline in performance.
  To address this limitation, we propose Hierarchical Graph Masked AutoEncoders (Hi-GMAE),
  a novel multi-scale GMAE framework designed to handle the hierarchical structures
  within graphs. First, Hi-GMAE constructs a multi-scale graph hierarchy through graph
  pooling, enabling the exploration of graph structures across different granularity
  levels. To ensure masking uniformity of subgraphs across these scales, we propose
  a novel coarse-to-fine strategy that initiates masking at the coarsest scale and
  progressively back-projects the mask to finer scales. Furthermore, we integrate
  a gradual recovery strategy with the masking process to mitigate the learning challenges
  posed by completely masked subgraphs. Diverging from the standard graph neural network
  (GNN) used in GMAE models, Hi-GMAE modifies its encoder and decoder into hierarchical
  structures. This entails using GNN at the finer scales for detailed local graph
  analysis and employing a graph transformer at coarser scales to capture global information.
  Such a design enables Hi-GMAE to effectively capture the multi-level information
  inherent in complex graph structures. Our experiments on 17 graph datasets, covering
  two graph learning tasks, consistently demonstrate that Hi-GMAE outperforms 29 state-of-the-art
  self-supervised competitors in capturing comprehensive graph information. Codes
  are available at.
codebase_url: https://github.com/LiuChuang0059/Hi-GMAE
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Hi-GMAE-F
mrr: 0.027
adjusted_mrr: 0.009
mrr_dataset_count: 1
benchmark_categories:
- Quantum Chemistry
benchmark_coverage:
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 1
  total: 3
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: QM7b
  rows:
  - model: DTNN
    model_key: dtnn
    model_plain: DTNN
    value: 0.074
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_display: Mar 2017
    date_iso: '2017-03-02'
    venue: Chemical Science
    codebase_url: https://github.com/deepchem/deepchem
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.074
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Multitask(CM)
    model_key: multitask(cm)
    model_plain: Multitask(CM)
    value: 0.086
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_display: Mar 2017
    date_iso: '2017-03-02'
    venue: Chemical Science
    codebase_url: https://github.com/deepchem/deepchem
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.086
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KRR(CM)
    model_key: krr(cm)
    model_plain: KRR(CM)
    value: 0.098
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_display: Mar 2017
    date_iso: '2017-03-02'
    venue: Chemical Science
    codebase_url: https://github.com/deepchem/deepchem
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.098
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Hi-GMAE-F
    model_key: hi-gmae-f
    model_plain: Hi-GMAE-F
    value: 74.4
    std: 1.9
    paper_value: 74.4
    paper_std: 1.9
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 17, 2024
    date_display: May 2024
    date_iso: '2024-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 74.4
    true_std: 1.9
    value_gap_source_arxiv: '2405.10642'
    value_gap_source_title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 74.4
    sort_std: 1.9
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 78.4
    std: 2.6
    paper_value: 78.4
    paper_std: 2.6
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: graphmae
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 17, 2024
    date_display: May 2024
    date_iso: '2024-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 78.4
    at_pub_std: 2.3
    at_pub_source_arxiv: '2310.14753'
    at_pub_source_title: Rethinking Tokenizer and Decoder in Masked Graph Modeling
      for Molecules
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-05-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 78.4
    true_std: 2.6
    value_gap_source_arxiv: '2405.10642'
    value_gap_source_title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 78.4
    sort_std: 2.6
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Mole-BERT
    model_key: mole-bert
    model_plain: Mole-BERT
    value: 79.8
    std: 2.6
    paper_value: 79.8
    paper_std: 2.6
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: molebert
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 17, 2024
    date_display: May 2024
    date_iso: '2024-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 79.8
    at_pub_std: 2.6
    at_pub_source_arxiv: '2310.14753'
    at_pub_source_title: Rethinking Tokenizer and Decoder in Masked Graph Modeling
      for Molecules
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-05-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 79.8
    true_std: 2.6
    value_gap_source_arxiv: '2405.10642'
    value_gap_source_title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 79.8
    sort_std: 2.6
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 80.4
    std: 3.3
    paper_value: 80.4
    paper_std: 3.3
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: graphCL
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 17, 2024
    date_display: May 2024
    date_iso: '2024-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 80.4
    at_pub_std: 3.3
    at_pub_source_arxiv: '2310.14753'
    at_pub_source_title: Rethinking Tokenizer and Decoder in Masked Graph Modeling
      for Molecules
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-05-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 80.4
    true_std: 3.3
    value_gap_source_arxiv: '2405.10642'
    value_gap_source_title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 80.4
    sort_std: 3.3
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 84.3
    std: 2.1
    paper_value: 84.3
    paper_std: 2.1
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: joao
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 17, 2024
    date_display: May 2024
    date_iso: '2024-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 84.3
    true_std: 2.1
    value_gap_source_arxiv: '2405.10642'
    value_gap_source_title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 84.3
    sort_std: 2.1
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ContextPred
    model_key: contextpred
    model_plain: ContextPred
    value: 88.3
    std: 0.5
    paper_value: 88.3
    paper_std: 0.5
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: pretrain-gnn
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 17, 2024
    date_display: May 2024
    date_iso: '2024-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 88.3
    true_std: 0.5
    value_gap_source_arxiv: '2405.10642'
    value_gap_source_title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 88.3
    sort_std: 0.5
    global_rank: 46
    paper_rank: 46
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AttrMask
    model_key: attrmask
    model_plain: AttrMask
    value: 109.5
    std: 7.6
    paper_value: 109.5
    paper_std: 7.6
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: pretrain-gnn
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 17, 2024
    date_display: May 2024
    date_iso: '2024-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 109.5
    true_std: 7.6
    value_gap_source_arxiv: '2405.10642'
    value_gap_source_title: 'Hi-GMAE: Hierarchical Graph Masked Autoencoders'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 109.5
    sort_std: 7.6
    global_rank: 52
    paper_rank: 52
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 122.9
    std: 2.2
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.12638'
    title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation'
    date: Feb 18, 2025
    date_display: Feb 2025
    date_iso: '2025-02-18'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/acharkq/NExT-Mol
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 60
    sort_value: 122.9
    sort_std: 2.2
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Quantum Chemistry
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Quantum Chemistry
    benchmark_slug: quantum-chemistry
    datasets:
    - dataset: QM7b
      dataset_slug: qm7b
single_proposed_model: Hi-GMAE-F
main_figure: /figures/2405.10642/main_figure.jpegoptim.jpg
---

