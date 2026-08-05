---
title: Federated Graph Classification over Non-IID Graphs
arxiv_id: '2106.13423'
source_url: ''
authors:
- name: Han Xie
  orcid: null
  s2_author_id: '2117714080'
  s2_url: null
- name: Jing Ma
  orcid: null
  s2_author_id: '2157405012'
  s2_url: null
- name: Li Xiong
  orcid: null
  s2_author_id: '2291135512'
  s2_url: null
- name: Carl Yang
  orcid: null
  s2_author_id: '1390553618'
  s2_url: null
published_date: Jun 25, 2021
published_date_iso: '2021-06-25'
published_venue: NeurIPS 2021
published_conference: NeurIPS 2021
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Federated learning has emerged as an important paradigm for training machine
  learning models in different domains. For graph-level tasks such as graph classification,
  graphs can also be regarded as a special type of data samples, which can be collected
  and stored in separate local systems. Similar to other domains, multiple local systems,
  each holding a small set of graphs, may benefit from collaboratively training a
  powerful graph mining model, such as the popular graph neural networks (GNNs). To
  provide more motivation towards such endeavors, we analyze real-world graphs from
  different domains to confirm that they indeed share certain graph properties that
  are statistically significant compared with random graphs. However, we also find
  that different sets of graphs, even from the same domain or same dataset, are non-IID
  regarding both graph structures and node features. To handle this, we propose a
  graph clustered federated learning (GCFL) framework that dynamically finds clusters
  of local systems based on the gradients of GNNs, and theoretically justify that
  such clusters can reduce the structure and feature heterogeneity among graphs owned
  by the local systems. Moreover, we observe the gradients of GNNs to be rather fluctuating
  in GCFL which impedes high-quality clustering, and design a gradient sequence-based
  clustering mechanism based on dynamic time warping (GCFL+). Extensive experimental
  results and in-depth analysis demonstrate the effectiveness of our proposed frameworks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCFL
mrr: 0.5011
adjusted_mrr: 0.3341
mrr_dataset_count: 2
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: IMDB-BINARY
  rows:
  - model: GCFL
    model_key: gcfl
    model_plain: GCFL
    value: 0.8299
    std: 0.052
    paper_value: 0.8299
    paper_std: 0.052
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average accuracy for 10 clients in single-dataset setting
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8299
    true_std: 0.052
    value_gap_source_arxiv: '2106.13423'
    value_gap_source_title: Federated Graph Classification over Non-IID Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8299
    sort_std: 0.052
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
  - model: DMoNPool-TIP
    model_key: gat +del-f
    model_plain: DMoNPool-TIP
    value: 0.7863
    std: 0.0054
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_display: Feb 2024
    date_iso: '2024-02-26'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7863
    sort_std: 0.0054
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DMoNPool-TIP
    model_key: graph transformer +del-f
    model_plain: DMoNPool-TIP
    value: 0.7828
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_display: Feb 2024
    date_iso: '2024-02-26'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7828
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FedProx
    model_key: fedprox
    model_plain: FedProx
    value: 0.7746
    std: 0.048
    paper_value: 0.7746
    paper_std: 0.048
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average accuracy for 10 clients in single-dataset setting
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7746
    true_std: 0.048
    value_gap_source_arxiv: '2106.13423'
    value_gap_source_title: Federated Graph Classification over Non-IID Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7746
    sort_std: 0.048
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
  - model: self-train
    model_key: self-train
    model_plain: self-train
    value: 0.7654
    std: 0.057
    paper_value: 0.7654
    paper_std: 0.057
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average accuracy for 10 clients in single-dataset setting
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7654
    true_std: 0.057
    value_gap_source_arxiv: '2106.13423'
    value_gap_source_title: Federated Graph Classification over Non-IID Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7654
    sort_std: 0.057
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FedAvg
    model_key: fedavg
    model_plain: FedAvg
    value: 0.7596
    std: 0.049
    paper_value: 0.7596
    paper_std: 0.049
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average accuracy for 10 clients in single-dataset setting
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7596
    true_std: 0.049
    value_gap_source_arxiv: '2106.13423'
    value_gap_source_title: Federated Graph Classification over Non-IID Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7596
    sort_std: 0.049
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: NCI1
  rows:
  - model: ECC
    model_key: wl-mlp
    model_plain: ECC
    value: 0.9954
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9954
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: gin
    model_plain: ECC
    value: 0.9934
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
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GNNs ... use node features
    is_global_top: true
    global_rank: 2
    sort_value: 0.9934
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ECC
    model_key: gcn
    model_plain: ECC
    value: 0.9727
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
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GNNs ... use node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.9727
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCFL
    model_key: gcfl
    model_plain: GCFL
    value: 0.7422
    std: 0.053
    paper_value: 0.7422
    paper_std: 0.053
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average accuracy for NCI1 (30 clients) in single-dataset-multi-client
      setting.
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7422
    true_std: 0.053
    value_gap_source_arxiv: '2106.13423'
    value_gap_source_title: Federated Graph Classification over Non-IID Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7422
    sort_std: 0.053
    global_rank: 452
    paper_rank: 452
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FedAvg
    model_key: fedavg
    model_plain: FedAvg
    value: 0.6474
    std: 0.076
    paper_value: 0.6474
    paper_std: 0.076
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average accuracy for NCI1 (30 clients) in single-dataset-multi-client
      setting.
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6474
    true_std: 0.076
    value_gap_source_arxiv: '2106.13423'
    value_gap_source_title: Federated Graph Classification over Non-IID Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6474
    sort_std: 0.076
    global_rank: 547
    paper_rank: 547
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: self-train
    model_key: self-train
    model_plain: self-train
    value: 0.6468
    std: 0.053
    paper_value: 0.6468
    paper_std: 0.053
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average accuracy for NCI1 (30 clients) in single-dataset-multi-client
      setting.
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6468
    true_std: 0.053
    value_gap_source_arxiv: '2106.13423'
    value_gap_source_title: Federated Graph Classification over Non-IID Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6468
    sort_std: 0.053
    global_rank: 548
    paper_rank: 548
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FedProx
    model_key: fedprox
    model_plain: FedProx
    value: 0.6437
    std: 0.072
    paper_value: 0.6437
    paper_std: 0.072
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average accuracy for NCI1 (30 clients) in single-dataset-multi-client
      setting.
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6437
    true_std: 0.072
    value_gap_source_arxiv: '2106.13423'
    value_gap_source_title: Federated Graph Classification over Non-IID Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6437
    sort_std: 0.072
    global_rank: 552
    paper_rank: 552
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: NCI1
      dataset_slug: nci1
    - dataset: IMDB-BINARY
      dataset_slug: imdb-binary
single_proposed_model: GCFL
main_figure: /figures/2106.13423/main_figure.jpegoptim.jpg
---

