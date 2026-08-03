---
title: Turning Tabular Foundation Models into Graph Foundation Models
arxiv_id: '2508.20906'
source_url: ''
authors:
- name: Dmitry Eremeev
  orcid: null
  s2_author_id: '2377795413'
  s2_url: null
- name: Gleb Bazhenov
  orcid: null
  s2_author_id: '2172208866'
  s2_url: null
- name: Oleg Platonov
  orcid: null
  s2_author_id: '2184723723'
  s2_url: null
- name: Artem Babenko
  orcid: null
  s2_author_id: '2377796287'
  s2_url: null
- name: Liudmila Prokhorenkova
  orcid: null
  s2_author_id: '2323374652'
  s2_url: null
published_date: Aug 28, 2025
published_date_iso: '2025-08-28'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: While foundation models have revolutionized such fields as natural language
  processing and computer vision, their potential in graph machine learning remains
  largely unexplored. One of the key challenges in designing graph foundation models
  (GFMs) is handling diverse node features that can vary across different graph datasets.
  While many works on GFMs have focused exclusively on text-attributed graphs, the
  problem of handling arbitrary features of other types in GFMs has not been fully
  addressed. However, this problem is not unique to the graph domain, as it also arises
  in the field of machine learning for tabular data. In this work, motivated by the
  recent success of tabular foundation models (TFMs) like TabPFNv2 or LimiX, we propose
  G2T-FM, a simple framework for turning tabular foundation models into graph foundation
  models. Specifically, G2T-FM augments the original node features with neighborhood
  feature aggregation, adds structural embeddings, and then applies a TFM to the constructed
  node representations. Even in a fully in-context regime, our model achieves strong
  results, significantly outperforming publicly available GFMs and performing competitively
  with, and often better than, well-tuned GNNs trained from scratch. Moreover, after
  finetuning, G2T-FM surpasses well-tuned GNN baselines. In particular, when combined
  with LimiX, G2T-FM often outperforms the best GNN by a significant margin. In summary,
  our paper reveals the potential of a previously overlooked direction of utilizing
  tabular foundation models for graph machine learning tasks..
codebase_url: https://github.com/yandex-research/G2T-FM
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
- Heterophilic Graphs
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 2
  total: 13
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
  dataset: Amazon2M
  rows:
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.4067
    std: 0.0053
    paper_value: 0.4067
    paper_std: 0.0053
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.953
    at_pub_std: null
    at_pub_source_arxiv: '2112.08331'
    at_pub_source_title: Model Stealing Attacks Against Inductive Graph Neural Networks
    at_pub_source_date_iso: '2021-12-15'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-12-15'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.5463
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.953
    true_std: null
    value_gap_source_arxiv: '2112.08331'
    value_gap_source_title: Model Stealing Attacks Against Inductive Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.5463
    has_value_note: false
    value_note: ''
    sort_value: 0.953
    sort_std: null
    global_rank: 1
    paper_rank: 69
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Model Stealing Attacks Against Inductive Graph Neural
      Networks
    comparison_source_arxiv: '2112.08331'
    is_best: true
    is_std_outlier: false
  - model: VecFormer
    model_key: sage
    model_plain: VecFormer
    value: 0.937
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
    arxiv_id: '2112.08331'
    title: Model Stealing Attacks Against Inductive Graph Neural Networks
    date: Dec 15, 2021
    date_display: Dec 2021
    date_iso: '2021-12-15'
    venue: IEEE Symposium on Security and Privacy
    codebase_url: https://github.com/xinleihe/GNNStealing
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.937
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VecFormer
    model_key: bgrl
    model_plain: VecFormer
    value: 0.932
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.21151'
    title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    date: Dec 30, 2024
    date_display: Dec 2024
    date_iso: '2024-12-30'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/iDEA-iSAIL-Lab-UIUC/pyg-ssl
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.932
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.4143
    std: 0.0046
    paper_value: 0.4143
    paper_std: 0.0046
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8651
    at_pub_std: 0.005
    at_pub_source_arxiv: '2212.07035'
    at_pub_source_title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive
      Learning'
    at_pub_source_date_iso: '2022-12-14'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-12-14'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.4508
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8651
    true_std: 0.005
    value_gap_source_arxiv: '2212.07035'
    value_gap_source_title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.4508
    has_value_note: false
    value_note: ''
    sort_value: 0.8651
    sort_std: 0.005
    global_rank: 18
    paper_rank: 66
    rank_delta: 48
    rank_delta_abs: 48
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive
      Learning'
    comparison_source_arxiv: '2212.07035'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.4007
    std: 0.005
    paper_value: 0.4007
    paper_std: 0.005
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.723
    at_pub_std: 0.01
    at_pub_source_arxiv: '2203.06389'
    at_pub_source_title: 'GRAND+: Scalable Graph Random Neural Networks'
    at_pub_source_date_iso: '2022-03-12'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-12'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.3223
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.723
    true_std: 0.01
    value_gap_source_arxiv: '2203.06389'
    value_gap_source_title: 'GRAND+: Scalable Graph Random Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.3223
    has_value_note: false
    value_note: ''
    sort_value: 0.723
    sort_std: 0.01
    global_rank: 37
    paper_rank: 69
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GRAND+: Scalable Graph Random Neural Networks'
    comparison_source_arxiv: '2203.06389'
    is_best: false
    is_std_outlier: false
  - model: G2T-LimiX (FT)
    model_key: g2t-limix (ft)
    model_plain: G2T-LimiX (FT)
    value: 0.4567
    std: 0.0035
    paper_value: 0.4567
    paper_std: 0.0035
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4567
    true_std: 0.0035
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4567
    sort_std: 0.0035
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: G2T-TabPFNv2 (FT)
    model_key: g2t-tabpfnv2 (ft)
    model_plain: G2T-TabPFNv2 (FT)
    value: 0.4471
    std: 0.0032
    paper_value: 0.4471
    paper_std: 0.0032
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4471
    true_std: 0.0032
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4471
    sort_std: 0.0032
    global_rank: 53
    paper_rank: 53
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TS-GNN (ICL)
    model_key: ts-gnn (icl)
    model_plain: TS-GNN (ICL)
    value: 0.43
    std: 0.0013
    paper_value: 0.43
    paper_std: 0.0013
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.43
    true_std: 0.0013
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.43
    sort_std: 0.0013
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.4156
    std: 0.0038
    paper_value: 0.4156
    paper_std: 0.0038
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4156
    true_std: 0.0038
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4156
    sort_std: 0.0038
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCOPE (FT)
    model_key: gcope (ft)
    model_plain: GCOPE (FT)
    value: 0.399
    std: 0.0043
    paper_value: 0.399
    paper_std: 0.0043
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.399
    true_std: 0.0043
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.399
    sort_std: 0.0043
    global_rank: 70
    paper_rank: 70
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AnyGraph (ICL)
    model_key: anygraph (icl)
    model_plain: AnyGraph (ICL)
    value: 0.3349
    std: 0.0344
    paper_value: 0.3349
    paper_std: 0.0344
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3349
    true_std: 0.0344
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3349
    sort_std: 0.0344
    global_rank: 75
    paper_rank: 75
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OpenGraph (ICL)
    model_key: opengraph (icl)
    model_plain: OpenGraph (ICL)
    value: 0.2936
    std: 0.0124
    paper_value: 0.2936
    paper_std: 0.0124
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=75)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on amazon-r. dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2936
    true_std: 0.0124
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2936
    sort_std: 0.0124
    global_rank: 77
    paper_rank: 77
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
  dataset: PubMed
  rows:
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: sagn
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.9517
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
    arxiv_id: '2605.24867'
    title: 'Clustering as Reasoning: A $k$-Means Interpretation of Chain-of-Thought
      Graph Learning'
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    venue: Accepted by ICML 2026
    codebase_url: https://github.com/Uncnbb/KCoT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9517
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: mixhop (lo)
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: graphsage (lo)
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.9511
    std: 0.0036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9511
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8604
    std: 0.0026
    paper_value: 0.8604
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8864
    at_pub_std: 0.003
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.025999999999999912
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9487
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.08829999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9487
    sort_std: null
    global_rank: 6
    paper_rank: 204
    rank_delta: 198
    rank_delta_abs: 198
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Non-backtracking Graph Neural Networks
    comparison_source_arxiv: '2310.07430'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8546
    std: 0.0018
    paper_value: 0.8546
    paper_std: 0.0018
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.889
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.034399999999999986
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9296
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07499999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: null
    global_rank: 17
    paper_rank: 216
    rank_delta: 199
    rank_delta_abs: 199
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Language is All a Graph Needs
    comparison_source_arxiv: '2308.07134'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8481
    std: 0.0022
    paper_value: 0.8481
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.884
    at_pub_std: null
    at_pub_source_arxiv: '2407.14996'
    at_pub_source_title: 'All Against Some: Efficient Integration of Large Language
      Models for Message Passing in Graph Neural Networks'
    at_pub_source_date_iso: '2024-07-20'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.03590000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9233
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07520000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: null
    global_rank: 19
    paper_rank: 233
    rank_delta: 214
    rank_delta_abs: 214
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'All Against Some: Efficient Integration of Large Language
      Models for Message Passing in Graph Neural Networks'
    comparison_source_arxiv: '2407.14996'
    is_best: false
    is_std_outlier: false
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.8495
    std: 0.0018
    paper_value: 0.8495
    paper_std: 0.0018
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8875
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03799999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8875
    true_std: 0.0016
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: 0.03799999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.8875
    sort_std: 0.0016
    global_rank: 110
    paper_rank: 230
    rank_delta: 120
    rank_delta_abs: 120
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Language is All a Graph Needs
    comparison_source_arxiv: '2308.07134'
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
  dataset: Questions
  rows:
  - model: topk
    model_key: mlp
    model_plain: topk
    value: 0.9733
    std: 0.0006
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2405.20445'
    title: Fully-inductive Node Classification on Arbitrary Graphs
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/DeepGraphLearning/GraphAny
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9733
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: topk
    model_key: ags-gnn
    model_plain: topk
    value: 0.9727
    std: 0.0004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: Feb 14, 2022
    date_display: Feb 2022
    date_iso: '2022-02-14'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9727
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.1542
    std: 0.0063
    paper_value: 0.1542
    paper_std: 0.0063
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9715
    at_pub_std: 0.0004
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.8173
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9715
    true_std: 0.0004
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.8173
    has_value_note: false
    value_note: ''
    sort_value: 0.9715
    sort_std: 0.0004
    global_rank: 3
    paper_rank: 150
    rank_delta: 147
    rank_delta_abs: 147
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    comparison_source_arxiv: '2405.20445'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.1675
    std: 0.0063
    paper_value: 0.1675
    paper_std: 0.0063
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9711
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.8036
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9711
    true_std: 0.0002
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.8036
    has_value_note: false
    value_note: ''
    sort_value: 0.9711
    sort_std: 0.0002
    global_rank: 4
    paper_rank: 150
    rank_delta: 146
    rank_delta_abs: 146
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    comparison_source_arxiv: '2405.20445'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.1655
    std: 0.0061
    paper_value: 0.1655
    paper_std: 0.0061
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7816
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.6161
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7816
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.6161
    has_value_note: false
    value_note: ''
    sort_value: 0.7816
    sort_std: null
    global_rank: 29
    paper_rank: 150
    rank_delta: 121
    rank_delta_abs: 121
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.1403
    std: 0.0086
    paper_value: 0.1403
    paper_std: 0.0086
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7795
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2405.16185'
    at_pub_source_title: Differentiable Cluster Graph Neural Network
    at_pub_source_date_iso: '2024-05-25'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.6392
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7795
    true_std: 0.0068
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.6392
    has_value_note: false
    value_note: ''
    sort_value: 0.7795
    sort_std: 0.0068
    global_rank: 34
    paper_rank: 150
    rank_delta: 116
    rank_delta_abs: 116
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Differentiable Cluster Graph Neural Network
    comparison_source_arxiv: '2405.16185'
    is_best: false
    is_std_outlier: false
  - model: G2T-LimiX (FT)
    model_key: g2t-limix (ft)
    model_plain: G2T-LimiX (FT)
    value: 0.2019
    std: 0.003
    paper_value: 0.2019
    paper_std: 0.003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
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
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2019
    true_std: 0.003
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2019
    sort_std: 0.003
    global_rank: 149
    paper_rank: 149
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: G2T-TabPFNv2 (FT)
    model_key: g2t-tabpfnv2 (ft)
    model_plain: G2T-TabPFNv2 (FT)
    value: 0.1907
    std: 0.0053
    paper_value: 0.1907
    paper_std: 0.0053
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
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
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1907
    true_std: 0.0053
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1907
    sort_std: 0.0053
    global_rank: 150
    paper_rank: 150
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCOPE (FT)
    model_key: gcope (ft)
    model_plain: GCOPE (FT)
    value: 0.0659
    std: 0.0043
    paper_value: 0.0659
    paper_std: 0.0043
    metric: ROC-AUC
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
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0659
    true_std: 0.0043
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0659
    sort_std: 0.0043
    global_rank: 151
    paper_rank: 151
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TS-GNN (ICL)
    model_key: ts-gnn (icl)
    model_plain: TS-GNN (ICL)
    value: 0.05
    std: 0.0048
    paper_value: 0.05
    paper_std: 0.0048
    metric: ROC-AUC
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
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.05
    true_std: 0.0048
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.05
    sort_std: 0.0048
    global_rank: 152
    paper_rank: 152
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AnyGraph (ICL)
    model_key: anygraph (icl)
    model_plain: AnyGraph (ICL)
    value: 0.0427
    std: 0.0066
    paper_value: 0.0427
    paper_std: 0.0066
    metric: ROC-AUC
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
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0427
    true_std: 0.0066
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0427
    sort_std: 0.0066
    global_rank: 153
    paper_rank: 153
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OpenGraph (ICL)
    model_key: opengraph (icl)
    model_plain: OpenGraph (ICL)
    value: 0.0377
    std: 0.0065
    paper_value: 0.0377
    paper_std: 0.0065
    metric: ROC-AUC
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
    protocol_note: Standard split for node classification on Questions dataset
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0377
    true_std: 0.0065
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0377
    sort_std: 0.0065
    global_rank: 154
    paper_rank: 154
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
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: Tolokers
  rows:
  - model: NodePFN
    model_key: polynormer-r
    model_plain: NodePFN
    value: 0.8591
    std: 0.0074
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/cornell-zhang/Polynormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8591
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: NodePFN
    model_key: nt
    model_plain: NodePFN
    value: 0.8569
    std: 0.0054
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2604.08980'
    title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware Graph
      Learning'
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    venue: arXiv.org
    codebase_url: https://github.com/cf020031308/MoNT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8569
    sort_std: 0.0054
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: NodePFN
    model_key: dir-nt
    model_plain: NodePFN
    value: 0.8502
    std: 0.0077
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.08980'
    title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware Graph
      Learning'
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    venue: arXiv.org
    codebase_url: https://github.com/cf020031308/MoNT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8502
    sort_std: 0.0077
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: G2T-LimiX (ICL)
    model_key: g2t-limix (icl)
    model_plain: G2T-LimiX (ICL)
    value: 0.6148
    std: 0.003
    paper_value: 0.6148
    paper_std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    variant_inference_reason: 'dataset: fuzzy match to tolokers (score=89)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: GraphLand benchmark, RL (random low) data split
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6148
    true_std: 0.003
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6148
    sort_std: 0.003
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
  - model: G2T-TabPFNv2 (ICL)
    model_key: g2t-tabpfnv2 (icl)
    model_plain: G2T-TabPFNv2 (ICL)
    value: 0.6042
    std: 0.0027
    paper_value: 0.6042
    paper_std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    variant_inference_reason: 'dataset: fuzzy match to tolokers (score=89)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: GraphLand benchmark, RL (random low) data split
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6042
    true_std: 0.0027
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6042
    sort_std: 0.0027
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OpenGraph (ICL)
    model_key: opengraph (icl)
    model_plain: OpenGraph (ICL)
    value: 0.4038
    std: 0.0113
    paper_value: 0.4038
    paper_std: 0.0113
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
    variant_inference_reason: 'dataset: fuzzy match to tolokers (score=89)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: GraphLand benchmark, RL (random low) data split
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4038
    true_std: 0.0113
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4038
    sort_std: 0.0113
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TS-GNN (ICL)
    model_key: ts-gnn (icl)
    model_plain: TS-GNN (ICL)
    value: 0.3854
    std: 0.0094
    paper_value: 0.3854
    paper_std: 0.0094
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
    variant_inference_reason: 'dataset: fuzzy match to tolokers (score=89)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: GraphLand benchmark, RL (random low) data split
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3854
    true_std: 0.0094
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3854
    sort_std: 0.0094
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCOPE (FT)
    model_key: gcope (ft)
    model_plain: GCOPE (FT)
    value: 0.2881
    std: 0.0128
    paper_value: 0.2881
    paper_std: 0.0128
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
    variant_inference_reason: 'dataset: fuzzy match to tolokers (score=89)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: GraphLand benchmark, RL (random low) data split
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2881
    true_std: 0.0128
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2881
    sort_std: 0.0128
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AnyGraph (ICL)
    model_key: anygraph (icl)
    model_plain: AnyGraph (ICL)
    value: 0.2875
    std: 0.0356
    paper_value: 0.2875
    paper_std: 0.0356
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
    variant_inference_reason: 'dataset: fuzzy match to tolokers (score=89)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: GraphLand benchmark, RL (random low) data split
    date: Aug 28, 2025
    date_display: Aug 2025
    date_iso: '2025-08-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2875
    true_std: 0.0356
    value_gap_source_arxiv: '2508.20906'
    value_gap_source_title: Turning Tabular Foundation Models into Graph Foundation
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2875
    sort_std: 0.0356
    global_rank: 30
    paper_rank: 30
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
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: Heterophilic Graphs
  datasets:
  - *id002
  - *id003
- benchmark: Other Graph Benchmarks
  datasets:
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: PubMed
      dataset_slug: pubmed
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Questions
      dataset_slug: questions
    - dataset: Tolokers
      dataset_slug: tolokers
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
---

