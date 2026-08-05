---
title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
arxiv_id: '2212.08665'
source_url: ''
authors:
- name: Yue Liu
  orcid: null
  s2_author_id: '2119034129'
  s2_url: null
- name: Xihong Yang
  orcid: null
  s2_author_id: '2154476091'
  s2_url: null
- name: Sihang Zhou
  orcid: null
  s2_author_id: '2516087'
  s2_url: null
- name: Xinwang Liu
  orcid: null
  s2_author_id: '2130021053'
  s2_url: null
- name: Zhen Wang
  orcid: null
  s2_author_id: '2144786408'
  s2_url: null
- name: K. Liang
  orcid: null
  s2_author_id: '2024445866'
  s2_url: null
- name: Wenxuan Tu
  orcid: null
  s2_author_id: '1381761887'
  s2_url: null
- name: Liangjun Li
  orcid: null
  s2_author_id: '2145729091'
  s2_url: null
- name: Jingcan Duan
  orcid: null
  s2_author_id: '2192715144'
  s2_url: null
- name: Cancan Chen
  orcid: null
  s2_author_id: '2175247410'
  s2_url: null
published_date: Dec 16, 2022
published_date_iso: '2022-12-16'
published_venue: AAAI 2022
published_conference: AAAI 2022
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Contrastive deep graph clustering, which aims to divide nodes into disjoint
  groups via contrastive mechanisms, is a challenging research spot. Among the recent
  works, hard sample mining-based algorithms have achieved great attention for their
  promising performance. However, we find that the existing hard sample mining methods
  have two problems as follows. 1) In the hardness measurement, the important structural
  information is overlooked for similarity calculation, degrading the representativeness
  of the selected hard negative samples. 2) Previous works merely focus on the hard
  negative sample pairs while neglecting the hard positive sample pairs. Nevertheless,
  samples within the same cluster but with low similarity should also be carefully
  learned. To solve the problems, we propose a novel contrastive deep graph clustering
  method dubbed Hard Sample Aware Network (HSAN) by introducing a comprehensive similarity
  measure criterion and a general dynamic sample weighing strategy. Concretely, in
  our algorithm, the similarities between samples are calculated by considering both
  the attribute embeddings and the structure embeddings, better revealing sample relationships
  and assisting hardness measurement. Moreover, under the guidance of the carefully
  collected high-confidence clustering information, our proposed weight modulating
  function will first recognize the positive and negative samples and then dynamically
  up-weight the hard sample pairs while down-weighting the easy ones. In this way,
  our method can mine not only the hard negative samples but also the hard positive
  sample, thus improving the discriminative capability of the samples further. Extensive
  experiments and analyses demonstrate the superiority and effectiveness of our proposed
  method. The source code of HSAN is shared at https://github.com/yueliu1999/HSAN
  and a collection (papers, codes and, datasets) of deep graph clustering is shared
  at https://github.com/yueliu1999/Awesome-Deep-Graph-Clustering on Github.
codebase_url: https://github.com/yueliu1999/HSAN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- HSAN
mrr: 0.27
adjusted_mrr: 0.18
mrr_dataset_count: 2
benchmark_categories:
- Hypergraph Benchmarks
benchmark_coverage:
- benchmark: Hypergraph Benchmarks
  benchmark_slug: hypergraph-benchmarks
  evaluated: 2
  total: 10
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: AMAP
  rows:
  - model: GANN
    model_key: gann
    model_plain: GANN
    value: 0.9405
    std: 0.0037
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9405
    sort_std: 0.0037
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.9308
    std: 0.0026
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9308
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9238
    std: 0.0014
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9238
    sort_std: 0.0014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8115
    std: 0.0105
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 14
    sort_value: 0.8115
    sort_std: 0.0105
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DCRN
    model_key: dcrn
    model_plain: DCRN
    value: 0.7086
    std: 0.0018
    paper_value: 0.7086
    paper_std: 0.0018
    metric: F1
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
    source_ref: AAAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7966
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08799999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7966
    true_std: 0.0025
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.08799999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7966
    sort_std: 0.0025
    global_rank: 15
    paper_rank: 26
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    value: 0.695
    std: 0.002
    paper_value: 0.695
    paper_std: 0.002
    metric: F1
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
    source_ref: AAAI 21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.76
    at_pub_std: 0.008
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06500000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.76
    true_std: 0.008
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.06500000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.008
    global_rank: 16
    paper_rank: 29
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: AGE
    model_key: age
    model_plain: AGE
    value: 0.6973
    std: 0.0024
    paper_value: 0.6973
    paper_std: 0.0024
    metric: F1
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
    source_ref: SIGKDD 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7174
    at_pub_std: 0.0093
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.020100000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7174
    true_std: 0.0093
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: 0.020100000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.7174
    sort_std: 0.0093
    global_rank: 24
    paper_rank: 29
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: HSAN
    model_key: hsan
    model_plain: HSAN
    value: 0.7115
    std: 0.008
    paper_value: 0.7115
    paper_std: 0.008
    metric: F1
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
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7115
    true_std: 0.008
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7115
    sort_std: 0.008
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
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    value: 0.6832
    std: 0.0183
    paper_value: 0.6832
    paper_std: 0.0183
    metric: F1
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
    source_ref: IJCAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7103
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.027100000000000013
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7103
    true_std: 0.0064
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: 0.027100000000000013
    has_value_note: false
    value_note: ''
    sort_value: 0.7103
    sort_std: 0.0064
    global_rank: 26
    paper_rank: 30
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.3145
    std: 0.0054
    paper_value: 0.3145
    paper_std: 0.0054
    metric: F1
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
    source_ref: AAAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6999
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.38539999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6999
    true_std: 0.0034
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: 0.38539999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.6999
    sort_std: 0.0034
    global_rank: 27
    paper_rank: 56
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.6454
    std: 0.0139
    paper_value: 0.6454
    paper_std: 0.0139
    metric: F1
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
    source_ref: IJCAI 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6987
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.053300000000000014
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6987
    true_std: 0.0054
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: 0.053300000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
    global_rank: 28
    paper_rank: 40
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: MGAE
    model_key: mgae
    model_plain: MGAE
    value: 0.6135
    std: 0.008
    paper_value: 0.6135
    paper_std: 0.008
    metric: F1
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
    source_ref: CIKM 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6808
    true_std: 0.0176
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: false
    value_gap: 0.06729999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.6808
    sort_std: 0.0176
    global_rank: 32
    paper_rank: 42
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.6596
    std: 0.0031
    paper_value: 0.6596
    paper_std: 0.0031
    metric: F1
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
    source_ref: WWW 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6805
    at_pub_std: 0.0181
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.02090000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6805
    true_std: 0.0181
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.02090000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.6805
    sort_std: 0.0181
    global_rank: 33
    paper_rank: 36
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    value: 0.6676
    std: 0.0067
    paper_value: 0.6676
    paper_std: 0.0067
    metric: F1
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
    source_ref: ICLR 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5447
    at_pub_std: 0.0083
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.12290000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6676
    true_std: 0.0067
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6676
    sort_std: 0.0067
    global_rank: 35
    paper_rank: 35
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
  - model: GDCL
    model_key: gdcl
    model_plain: GDCL
    value: 0.6639
    std: 0.0065
    paper_value: 0.6639
    paper_std: 0.0065
    metric: F1
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
    source_ref: IJCAI 21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6639
    true_std: 0.0065
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6639
    sort_std: 0.0065
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.6592
    std: 0.008
    paper_value: 0.6592
    paper_std: 0.008
    metric: F1
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
    source_ref: ICML 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6592
    true_std: 0.008
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6592
    sort_std: 0.008
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
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.6107
    std: 0.0049
    paper_value: 0.6107
    paper_std: 0.0049
    metric: F1
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
    source_ref: IJCAI 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6483
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.03759999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6483
    true_std: 0.0059
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.03759999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6483
    sort_std: 0.0059
    global_rank: 40
    paper_rank: 42
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.6283
    std: 0.0159
    paper_value: 0.6283
    paper_std: 0.0159
    metric: F1
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
    source_ref: ICML 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4273
    at_pub_std: 0.0102
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.20099999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6283
    true_std: 0.0159
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6283
    sort_std: 0.0159
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: EAT
  rows:
  - model: HSAN
    model_key: hsan
    model_plain: HSAN
    value: 0.7702
    std: 0.0033
    paper_value: 0.7702
    paper_std: 0.0033
    metric: F1
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
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7702
    true_std: 0.0033
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7702
    sort_std: 0.0033
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
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.7702
    std: 0.0033
    paper_value: 0.7702
    paper_std: 0.0033
    metric: F1
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
    source_ref: ICML 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7702
    true_std: 0.0033
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7702
    sort_std: 0.0033
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
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    value: 0.7682
    std: 0.0023
    paper_value: 0.7682
    paper_std: 0.0023
    metric: F1
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
    source_ref: AAAI 21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7125
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.05569999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7682
    true_std: 0.0023
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7682
    sort_std: 0.0023
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: true
    is_std_outlier: false
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    value: 0.7681
    std: 0.0145
    paper_value: 0.7681
    paper_std: 0.0145
    metric: F1
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
    source_ref: IJCAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.352
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.4161
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7681
    true_std: 0.0145
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7681
    sort_std: 0.0145
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: true
    is_std_outlier: false
  - model: AGE
    model_key: age
    model_plain: AGE
    value: 0.7598
    std: 0.0068
    paper_value: 0.7598
    paper_std: 0.0068
    metric: F1
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
    source_ref: SIGKDD 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7174
    at_pub_std: 0.0093
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.04239999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7598
    true_std: 0.0068
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7598
    sort_std: 0.0068
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.7596
    std: 0.0023
    paper_value: 0.7596
    paper_std: 0.0023
    metric: F1
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
    source_ref: IJCAI 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6987
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.060900000000000065
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7596
    true_std: 0.0023
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7596
    sort_std: 0.0023
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: DCRN
    model_key: dcrn
    model_plain: DCRN
    value: 0.7551
    std: 0.0077
    paper_value: 0.7551
    paper_std: 0.0077
    metric: F1
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
    source_ref: AAAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4706
    at_pub_std: 0.0066
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2845
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7551
    true_std: 0.0077
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7551
    sort_std: 0.0077
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
  - model: MGAE
    model_key: mgae
    model_plain: MGAE
    value: 0.7157
    std: 0.0248
    paper_value: 0.7157
    paper_std: 0.0248
    metric: F1
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
    source_ref: CIKM 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7157
    true_std: 0.0248
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7157
    sort_std: 0.0248
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
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.6928
    std: 0.023
    paper_value: 0.6928
    paper_std: 0.023
    metric: F1
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
    source_ref: IJCAI 19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.643
    at_pub_std: 0.0195
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.049799999999999955
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6928
    true_std: 0.023
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6928
    sort_std: 0.023
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    value: 0.5455
    std: 0.0097
    paper_value: 0.5455
    paper_std: 0.0097
    metric: F1
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
    source_ref: ICLR 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.2182
    at_pub_std: 0.0098
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.3273
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5455
    true_std: 0.0097
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5455
    sort_std: 0.0097
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.5344
    std: 0.0081
    paper_value: 0.5344
    paper_std: 0.0081
    metric: F1
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
    source_ref: WWW 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5066
    at_pub_std: 0.0149
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.027799999999999936
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5344
    true_std: 0.0081
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5344
    sort_std: 0.0081
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: GDCL
    model_key: gdcl
    model_plain: GDCL
    value: 0.5153
    std: 0.0038
    paper_value: 0.5153
    paper_std: 0.0038
    metric: F1
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
    source_ref: IJCAI 21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5153
    true_std: 0.0038
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5153
    sort_std: 0.0038
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.4107
    std: 0.0312
    paper_value: 0.4107
    paper_std: 0.0312
    metric: F1
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
    source_ref: ICML 20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3288
    at_pub_std: 0.055
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.08190000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.47
    true_std: 0.06
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.059299999999999964
    has_value_note: false
    value_note: ''
    sort_value: 0.47
    sort_std: 0.06
    global_rank: 23
    paper_rank: 28
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.4375
    std: 0.0078
    paper_value: 0.4375
    paper_std: 0.0078
    metric: F1
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
    source_ref: AAAI 22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3053
    at_pub_std: 0.0147
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.13219999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4375
    true_std: 0.0078
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4375
    sort_std: 0.0078
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Hypergraph Benchmarks
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Hypergraph Benchmarks
    benchmark_slug: hypergraph-benchmarks
    datasets:
    - dataset: AMAP
      dataset_slug: amap
    - dataset: EAT
      dataset_slug: eat
single_proposed_model: HSAN
main_figure: /figures/2212.08665/main_figure.jpegoptim.jpg
---

