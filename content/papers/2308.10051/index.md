---
title: 'The Snowflake Hypothesis: Training Deep GNN with One Node One Receptive field'
arxiv_id: '2308.10051'
source_url: ''
authors:
- name: Kun Wang
  orcid: null
  s2_author_id: '2119043696'
  s2_url: null
- name: Guohao Li
  orcid: null
  s2_author_id: '1669997484'
  s2_url: null
- name: Shilong Wang
  orcid: null
  s2_author_id: '2274309064'
  s2_url: null
- name: Guibin Zhang
  orcid: null
  s2_author_id: '2232926268'
  s2_url: null
- name: K. Wang
  orcid: null
  s2_author_id: '40636684'
  s2_url: null
- name: Yang You
  orcid: null
  s2_author_id: '2147330258'
  s2_url: null
- name: Xiaojiang Peng
  orcid: null
  s2_author_id: '1766837'
  s2_url: null
- name: Yuxuan Liang
  orcid: null
  s2_author_id: '3431194'
  s2_url: null
- name: Yang Wang
  orcid: null
  s2_author_id: '2256978969'
  s2_url: null
published_date: Aug 19, 2023
published_date_iso: '2023-08-19'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Despite Graph Neural Networks (GNNs) demonstrating considerable promise
  in graph representation learning tasks, GNNs predominantly face significant issues
  with over-fitting and over-smoothing as they go deeper as models of computer vision
  (CV) realm. Given that the potency of numerous CV and language models is attributable
  to that support reliably training very deep architectures, we conduct a systematic
  study of deeper GNN research trajectories. Our findings indicate that the current
  success of deep GNNs primarily stems from (I) the adoption of innovations from CNNs,
  such as residual/skip connections, or (II) the tailor-made aggregation algorithms
  like DropEdge. However, these algorithms often lack intrinsic interpretability and
  indiscriminately treat all nodes within a given layer in a similar manner, thereby
  failing to capture the nuanced differences among various nodes. In this paper, we
  introduce the Snowflake Hypothesis -- a novel paradigm underpinning the concept
  of ``one node, one receptive field''''. The hypothesis draws inspiration from the
  unique and individualistic patterns of each snowflake, proposing a corresponding
  uniqueness in the receptive fields of nodes in the GNNs. We employ the simplest
  gradient and node-level cosine distance as guiding principles to regulate the aggregation
  depth for each node, and conduct comprehensive experiments including: (1) different
  training scheme; (2) various shallow and deep GNN backbones, especially on deep
  frameworks such as JKNet, ResGCN, PairNorm etc. (3) various numbers of layers (8,
  16, 32, 64) on multiple benchmarks (six graphs including dense graphs with millions
  of nodes); (4) compare with different aggregation strategies. The observational
  results demonstrate that our framework can serve as a universal operator for a range
  of tasks, and it displays tremendous potential on deep GNNs. It can be applied to
  various GNN frameworks, enhancing its effectiveness when operating in-depth, and
  guiding the selection of the optimal network depth in an explainable and generalizable
  way.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7339
    std: null
    paper_value: 0.7339
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to citeseer (score=94)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) with 8 layers
    date: Aug 19, 2023
    date_display: Aug 2023
    date_iso: '2023-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7943
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.06040000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8033
    true_std: 0.0088
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.06940000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8033
    sort_std: 0.0088
    global_rank: 37
    paper_rank: 275
    rank_delta: 238
    rank_delta_abs: 238
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.7134
    std: null
    paper_value: 0.7134
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to citeseer (score=94)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) with 8 layers
    date: Aug 19, 2023
    date_display: Aug 2023
    date_iso: '2023-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7843
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-25'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.07089999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7843
    true_std: 0.0031
    value_gap_source_arxiv: '2110.13094'
    value_gap_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.07089999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.7843
    sort_std: 0.0031
    global_rank: 64
    paper_rank: 517
    rank_delta: 453
    rank_delta_abs: 453
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: SnoHv2
    model_key: snohv2
    model_plain: SnoHv2
    value: 0.7324
    std: null
    paper_value: 0.7324
    paper_std: null
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
    variant_inference_reason: 'dataset: fuzzy match to citeseer (score=94)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) with 8 layers
    date: Aug 19, 2023
    date_display: Aug 2023
    date_iso: '2023-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-19'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7324
    true_std: null
    value_gap_source_arxiv: '2308.10051'
    value_gap_source_title: 'The Snowflake Hypothesis: Training Deep GNN with One
      Node One Receptive field'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7324
    sort_std: null
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
  - model: ResGCN
    model_key: resgcn
    model_plain: ResGCN
    value: 0.7201
    std: null
    paper_value: 0.7201
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to citeseer (score=94)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) with 32 layers
    date: Aug 19, 2023
    date_display: Aug 2023
    date_iso: '2023-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.708
    at_pub_std: 0.007
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2023-08-19'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0121
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7201
    true_std: null
    value_gap_source_arxiv: '2308.10051'
    value_gap_source_title: 'The Snowflake Hypothesis: Training Deep GNN with One
      Node One Receptive field'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7201
    sort_std: null
    global_rank: 447
    paper_rank: 447
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: UGS(IPR=5%)
    model_key: ugs(ipr=5%)
    model_plain: UGS(IPR=5%)
    value: 0.658
    std: null
    paper_value: 0.658
    paper_std: null
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
    variant_inference_reason: 'dataset: fuzzy match to citeseer (score=94)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) with 8 layers
    date: Aug 19, 2023
    date_display: Aug 2023
    date_iso: '2023-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-19'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.658
    true_std: null
    value_gap_source_arxiv: '2308.10051'
    value_gap_source_title: 'The Snowflake Hypothesis: Training Deep GNN with One
      Node One Receptive field'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.658
    sort_std: null
    global_rank: 723
    paper_rank: 723
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RP
    model_key: rp
    model_plain: RP
    value: 0.455
    std: null
    paper_value: 0.455
    paper_std: null
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
    variant_inference_reason: 'dataset: fuzzy match to citeseer (score=94)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) with 8 layers
    date: Aug 19, 2023
    date_display: Aug 2023
    date_iso: '2023-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-19'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.455
    true_std: null
    value_gap_source_arxiv: '2308.10051'
    value_gap_source_title: 'The Snowflake Hypothesis: Training Deep GNN with One
      Node One Receptive field'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.455
    sort_std: null
    global_rank: 830
    paper_rank: 830
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: CiteSeer
      dataset_slug: citeseer
---

