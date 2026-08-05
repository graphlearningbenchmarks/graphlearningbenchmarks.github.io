---
title: Reconstruction for Powerful Graph Representations
arxiv_id: '2110.00577'
source_url: ''
authors:
- name: Leonardo Cotta
  orcid: null
  s2_author_id: '113902542'
  s2_url: null
- name: Christopher Morris
  orcid: null
  s2_author_id: '143622465'
  s2_url: null
- name: Bruno Ribeiro
  orcid: null
  s2_author_id: '145617731'
  s2_url: null
published_date: Oct 1, 2021
published_date_iso: '2021-10-01'
published_venue: NeurIPS 2021
published_conference: NeurIPS 2021
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Graph neural networks (GNNs) have limited expressive power, failing to represent
  many graph classes correctly. While more expressive graph representation learning
  (GRL) alternatives can distinguish some of these classes, they are significantly
  harder to implement, may not scale well, and have not been shown to outperform well-tuned
  GNNs in real-world tasks. Thus, devising simple, scalable, and expressive GRL architectures
  that also achieve real-world improvements remains an open challenge. In this work,
  we show the extent to which graph reconstruction---reconstructing a graph from its
  subgraphs---can mitigate the theoretical and practical problems currently faced
  by GRL architectures. First, we leverage graph reconstruction to build two new classes
  of expressive graph representations. Secondly, we show how graph reconstruction
  boosts the expressive power of any GNN architecture while being a (provably) powerful
  inductive bias for invariances to vertex removals. Empirically, we show how reconstruction
  can boost GNN's expressive power---while maintaining its invariance to permutations
  of the vertices---by solving seven graph property tasks not solvable by the original
  GNN. Further, we demonstrate how it boosts state-of-the-art GNN's performance across
  nine real-world benchmark datasets.
codebase_url: https://github.com/PurdueMINDS/reconstruction-gnns
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
- MoleculeNet
- GNNBenchmark
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 2
  total: 16
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 1
  total: 9
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id004
  dataset: CSL
  rows:
  - model: Reconstr. (n-1)
    model_key: reconstr. (n-1)
    model_plain: Reconstr. (n-1)
    value: 1.0
    std: 0.0
    paper_value: 1.0
    paper_std: 0.0
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 5-fold cross validation as per original work
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0
    true_std: 0.0
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0
    sort_std: 0.0
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
  - model: GPM
    model_key: ppgn
    model_plain: GPM
    value: 1.0
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
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: rw-agentnet
    model_plain: GPM
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: agentnet
    model_plain: GPM
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Positional GIN
    model_key: positional gin
    model_plain: Positional GIN
    value: 0.9933
    std: 0.0133
    paper_value: 0.9933
    paper_std: 0.0133
    metric: Accuracy
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Uses Laplacian embeddings as positional features
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9933
    true_std: 0.0133
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9933
    sort_std: 0.0133
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PPGN (3-WL)
    model_key: ppgn (3-wl)
    model_plain: PPGN (3-WL)
    value: 0.978
    std: 0.1091
    paper_value: 0.978
    paper_std: 0.1091
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 5-fold cross validation as per original work
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.978
    true_std: 0.1091
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.978
    sort_std: 0.1091
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Ring-GNN
    model_key: ring-gnn
    model_plain: Ring-GNN
    value: 0.1
    std: 0.0
    paper_value: 0.1
    paper_std: 0.0
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 5-fold cross validation as per original work
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.8
    at_pub_std: 0.157
    at_pub_source_arxiv: '1905.12560'
    at_pub_source_title: On the Equivalence between Graph Isomorphism Testing and
      Function Approximation with GNNs
    at_pub_source_date_iso: '2019-05-29'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2019-05-29'
    value_gap_source_date_label: NeurIPS 2019
    gap_vs_at_pub: 0.7000000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8
    true_std: 0.157
    value_gap_source_arxiv: '1905.12560'
    value_gap_source_title: On the Equivalence between Graph Isomorphism Testing and
      Function Approximation with GNNs
    value_gap_source_is_current_paper: false
    value_gap: 0.7000000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.157
    global_rank: 58
    paper_rank: 79
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Equivalence between Graph Isomorphism Testing
      and Function Approximation with GNNs
    comparison_source_arxiv: '1905.12560'
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (ceil(n/2))
    model_key: reconstr. (ceil(n/2))
    model_plain: Reconstr. (ceil(n/2))
    value: 0.4933
    std: 0.0742
    paper_value: 0.4933
    paper_std: 0.0742
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 5-fold cross validation as per original work
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4933
    true_std: 0.0742
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4933
    sort_std: 0.0742
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA (orig.)
    model_key: pna (orig.)
    model_plain: PNA (orig.)
    value: 0.1
    std: 0.0298
    paper_value: 0.1
    paper_std: 0.0298
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 5-fold cross validation as per original work
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1
    true_std: 0.0298
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1
    sort_std: 0.0298
    global_rank: 82
    paper_rank: 82
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN (orig.)
    model_key: gcn (orig.)
    model_plain: GCN (orig.)
    value: 0.0666
    std: 0.021
    paper_value: 0.0666
    paper_std: 0.021
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 5-fold cross validation as per original work
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0666
    true_std: 0.021
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0666
    sort_std: 0.021
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN (orig.)
    model_key: gin (orig.)
    model_plain: GIN (orig.)
    value: 0.0466
    std: 0.04
    paper_value: 0.0466
    paper_std: 0.04
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 5-fold cross validation as per original work
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0466
    true_std: 0.04
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0466
    sort_std: 0.04
    global_rank: 98
    paper_rank: 98
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
  - model: Reconstr. (ceil(n/2)) [GIN]
    model_key: reconstr. (ceil(n/2)) [gin]
    model_plain: Reconstr. (ceil(n/2)) [GIN]
    value: 0.744
    std: 0.0075
    paper_value: 0.744
    paper_std: 0.0075
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC reported as percentage in table; converted to [0,1]
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.744
    true_std: 0.0075
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.744
    sort_std: 0.0075
    global_rank: 242
    paper_rank: 242
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (ceil(n/2)) [GCN]
    model_key: reconstr. (ceil(n/2)) [gcn]
    model_plain: Reconstr. (ceil(n/2)) [GCN]
    value: 0.7403
    std: 0.0063
    paper_value: 0.7403
    paper_std: 0.0063
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC reported as percentage in table; converted to [0,1]
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7403
    true_std: 0.0063
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7403
    sort_std: 0.0063
    global_rank: 258
    paper_rank: 258
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (ceil(n/2)) [PNA]
    model_key: reconstr. (ceil(n/2)) [pna]
    model_plain: Reconstr. (ceil(n/2)) [PNA]
    value: 0.7371
    std: 0.0061
    paper_value: 0.7371
    paper_std: 0.0061
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC reported as percentage in table; converted to [0,1]
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7371
    true_std: 0.0061
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7371
    sort_std: 0.0061
    global_rank: 263
    paper_rank: 263
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-2) [GIN]
    model_key: reconstr. (n-2) [gin]
    model_plain: Reconstr. (n-2) [GIN]
    value: 0.6536
    std: 0.0049
    paper_value: 0.6536
    paper_std: 0.0049
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6536
    true_std: 0.0049
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6536
    sort_std: 0.0049
    global_rank: 315
    paper_rank: 315
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-2) [PNA]
    model_key: reconstr. (n-2) [pna]
    model_plain: Reconstr. (n-2) [PNA]
    value: 0.6522
    std: 0.0047
    paper_value: 0.6522
    paper_std: 0.0047
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6522
    true_std: 0.0047
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6522
    sort_std: 0.0047
    global_rank: 317
    paper_rank: 317
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-3) [PNA]
    model_key: reconstr. (n-3) [pna]
    model_plain: Reconstr. (n-3) [PNA]
    value: 0.6503
    std: 0.0058
    paper_value: 0.6503
    paper_std: 0.0058
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6503
    true_std: 0.0058
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6503
    sort_std: 0.0058
    global_rank: 319
    paper_rank: 319
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-3) [GIN]
    model_key: reconstr. (n-3) [gin]
    model_plain: Reconstr. (n-3) [GIN]
    value: 0.6484
    std: 0.0071
    paper_value: 0.6484
    paper_std: 0.0071
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6484
    true_std: 0.0071
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6484
    sort_std: 0.0071
    global_rank: 320
    paper_rank: 320
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-3) [GCN]
    model_key: reconstr. (n-3) [gcn]
    model_plain: Reconstr. (n-3) [GCN]
    value: 0.647
    std: 0.0081
    paper_value: 0.647
    paper_std: 0.0081
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.647
    true_std: 0.0081
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.647
    sort_std: 0.0081
    global_rank: 322
    paper_rank: 322
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-1) [GCN]
    model_key: reconstr. (n-1) [gcn]
    model_plain: Reconstr. (n-1) [GCN]
    value: 0.6451
    std: 0.006
    paper_value: 0.6451
    paper_std: 0.006
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6451
    true_std: 0.006
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6451
    sort_std: 0.006
    global_rank: 323
    paper_rank: 323
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-2) [GCN]
    model_key: reconstr. (n-2) [gcn]
    model_plain: Reconstr. (n-2) [GCN]
    value: 0.6438
    std: 0.0039
    paper_value: 0.6438
    paper_std: 0.0039
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6438
    true_std: 0.0039
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6438
    sort_std: 0.0039
    global_rank: 324
    paper_rank: 324
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-1) [PNA]
    model_key: reconstr. (n-1) [pna]
    model_plain: Reconstr. (n-1) [PNA]
    value: 0.6414
    std: 0.0076
    paper_value: 0.6414
    paper_std: 0.0076
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6414
    true_std: 0.0076
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6414
    sort_std: 0.0076
    global_rank: 326
    paper_rank: 326
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-1) [GIN]
    model_key: reconstr. (n-1) [gin]
    model_plain: Reconstr. (n-1) [GIN]
    value: 0.6395
    std: 0.0053
    paper_value: 0.6395
    paper_std: 0.0053
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6395
    true_std: 0.0053
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6395
    sort_std: 0.0053
    global_rank: 329
    paper_rank: 329
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN (orig.)
    model_key: gcn (orig.)
    model_plain: GCN (orig.)
    value: 0.6354
    std: 0.0042
    paper_value: 0.6354
    paper_std: 0.0042
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6354
    true_std: 0.0042
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6354
    sort_std: 0.0042
    global_rank: 332
    paper_rank: 332
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN (orig.)
    model_key: gin (orig.)
    model_plain: GIN (orig.)
    value: 0.6341
    std: 0.0074
    paper_value: 0.6341
    paper_std: 0.0074
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6341
    true_std: 0.0074
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6341
    sort_std: 0.0074
    global_rank: 333
    paper_rank: 333
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA (orig.)
    model_key: pna (orig.)
    model_plain: PNA (orig.)
    value: 0.6269
    std: 0.0063
    paper_value: 0.6269
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-moltox21 (score=79)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6269
    true_std: 0.0063
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6269
    sort_std: 0.0063
    global_rank: 335
    paper_rank: 335
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
- &id001
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
  - model: GIN (n-2)
    model_key: gin (n-2)
    model_plain: GIN (n-2)
    value: 0.7753
    std: 0.0159
    paper_value: 0.7753
    paper_std: 0.0159
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
    table_ref: further results
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC reported as percentage in table, normalized to [0, 1]
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7753
    true_std: 0.0159
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7753
    sort_std: 0.0159
    global_rank: 130
    paper_rank: 130
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN (n-1)
    model_key: gcn (n-1)
    model_plain: GCN (n-1)
    value: 0.7683
    std: 0.0188
    paper_value: 0.7683
    paper_std: 0.0188
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
    table_ref: further results
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC reported as percentage in table, normalized to [0, 1]
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7683
    true_std: 0.0188
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7683
    sort_std: 0.0188
    global_rank: 176
    paper_rank: 176
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA (n-3)
    model_key: pna (n-3)
    model_plain: PNA (n-3)
    value: 0.751
    std: 0.0073
    paper_value: 0.751
    paper_std: 0.0073
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC reported as percentage in table, normalized to [0, 1]
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.751
    true_std: 0.0073
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.751
    sort_std: 0.0073
    global_rank: 251
    paper_rank: 251
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN (ceil(n/2))
    model_key: gin (ceil(n/2))
    model_plain: GIN (ceil(n/2))
    value: 0.744
    std: 0.0075
    paper_value: 0.744
    paper_std: 0.0075
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC reported as percentage in table, normalized to [0, 1]
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.744
    true_std: 0.0075
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.744
    sort_std: 0.0075
    global_rank: 267
    paper_rank: 267
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN (ceil(n/2))
    model_key: gcn (ceil(n/2))
    model_plain: GCN (ceil(n/2))
    value: 0.7403
    std: 0.0063
    paper_value: 0.7403
    paper_std: 0.0063
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC reported as percentage in table, normalized to [0, 1]
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7403
    true_std: 0.0063
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7403
    sort_std: 0.0063
    global_rank: 275
    paper_rank: 275
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA (ceil(n/2))
    model_key: pna (ceil(n/2))
    model_plain: PNA (ceil(n/2))
    value: 0.7371
    std: 0.0061
    paper_value: 0.7371
    paper_std: 0.0061
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC reported as percentage in table, normalized to [0, 1]
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7371
    true_std: 0.0061
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7371
    sort_std: 0.0061
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
  dataset: ogbg-molpcba
  rows:
  - model: SigGate-GT
    model_key: hig with graphormer
    model_plain: SigGate-GT
    value: 0.3167
    std: 0.0034
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.11678'
    title: Compressing Deep Graph Neural Networks via Adversarial Knowledge Distillation
    date: May 24, 2022
    date_display: May 2022
    date_iso: '2022-05-24'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/TencentYoutuResearch/HIG-GraphClassification
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.3167
    sort_std: 0.0034
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: grpe-large
    model_plain: SigGate-GT
    value: 0.315
    std: 0.001
    metric: AP
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.315
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: graphormer
    model_plain: SigGate-GT
    value: 0.314
    std: null
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2207.08806'
    title: Unified 2D and 3D Pre-Training of Molecular Representations
    date: Jul 14, 2022
    date_display: Jul 2022
    date_iso: '2022-07-14'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/teslacool/UnifiedMolPretrain
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.314
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PNA (orig.)
    model_key: pna (orig.)
    model_plain: PNA (orig.)
    value: 0.2545
    std: 0.0004
    paper_value: 0.2545
    paper_std: 0.0004
    metric: AP
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2545
    true_std: 0.0004
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2545
    sort_std: 0.0004
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
  - model: Reconstr. (n-1) [GIN]
    model_key: reconstr. (n-1) [gin]
    model_plain: Reconstr. (n-1) [GIN]
    value: 0.236
    std: 0.0002
    paper_value: 0.236
    paper_std: 0.0002
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.236
    true_std: 0.0002
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.236
    sort_std: 0.0002
    global_rank: 88
    paper_rank: 88
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-3) [GIN]
    model_key: reconstr. (n-3) [gin]
    model_plain: Reconstr. (n-3) [GIN]
    value: 0.2333
    std: 0.0009
    paper_value: 0.2333
    paper_std: 0.0009
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2333
    true_std: 0.0009
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2333
    sort_std: 0.0009
    global_rank: 90
    paper_rank: 90
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-2) [GIN]
    model_key: reconstr. (n-2) [gin]
    model_plain: Reconstr. (n-2) [GIN]
    value: 0.2325
    std: 0.0
    paper_value: 0.2325
    paper_std: 0.0
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2325
    true_std: 0.0
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2325
    sort_std: 0.0
    global_rank: 92
    paper_rank: 92
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-1) [PNA]
    model_key: reconstr. (n-1) [pna]
    model_plain: Reconstr. (n-1) [PNA]
    value: 0.2311
    std: 0.0005
    paper_value: 0.2311
    paper_std: 0.0005
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2311
    true_std: 0.0005
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2311
    sort_std: 0.0005
    global_rank: 93
    paper_rank: 93
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-2) [PNA]
    model_key: reconstr. (n-2) [pna]
    model_plain: Reconstr. (n-2) [PNA]
    value: 0.221
    std: 0.0003
    paper_value: 0.221
    paper_std: 0.0003
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.221
    true_std: 0.0003
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.221
    sort_std: 0.0003
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-1) [GCN]
    model_key: reconstr. (n-1) [gcn]
    model_plain: Reconstr. (n-1) [GCN]
    value: 0.2125
    std: 0.0025
    paper_value: 0.2125
    paper_std: 0.0025
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2125
    true_std: 0.0025
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2125
    sort_std: 0.0025
    global_rank: 100
    paper_rank: 100
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN (orig.)
    model_key: gin (orig.)
    model_plain: GIN (orig.)
    value: 0.2116
    std: 0.0028
    paper_value: 0.2116
    paper_std: 0.0028
    metric: AP
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2116
    true_std: 0.0028
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2116
    sort_std: 0.0028
    global_rank: 102
    paper_rank: 102
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN (orig.)
    model_key: gcn (orig.)
    model_plain: GCN (orig.)
    value: 0.202
    std: 0.0024
    paper_value: 0.202
    paper_std: 0.0024
    metric: AP
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.202
    true_std: 0.0024
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.202
    sort_std: 0.0024
    global_rank: 104
    paper_rank: 104
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-2) [GCN]
    model_key: reconstr. (n-2) [gcn]
    model_plain: Reconstr. (n-2) [GCN]
    value: 0.201
    std: 0.0008
    paper_value: 0.201
    paper_std: 0.0008
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.201
    true_std: 0.0008
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.201
    sort_std: 0.0008
    global_rank: 105
    paper_rank: 105
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-3) [PNA]
    model_key: reconstr. (n-3) [pna]
    model_plain: Reconstr. (n-3) [PNA]
    value: 0.2005
    std: 0.0015
    paper_value: 0.2005
    paper_std: 0.0015
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2005
    true_std: 0.0015
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2005
    sort_std: 0.0015
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (n-3) [GCN]
    model_key: reconstr. (n-3) [gcn]
    model_plain: Reconstr. (n-3) [GCN]
    value: 0.1904
    std: 0.0003
    paper_value: 0.1904
    paper_std: 0.0003
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1904
    true_std: 0.0003
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1904
    sort_std: 0.0003
    global_rank: 107
    paper_rank: 107
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (ceil(n/2)) [GIN]
    model_key: reconstr. (ceil(n/2)) [gin]
    model_plain: Reconstr. (ceil(n/2)) [GIN]
    value: 0.135
    std: 0.0032
    paper_value: 0.135
    paper_std: 0.0032
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.135
    true_std: 0.0032
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.135
    sort_std: 0.0032
    global_rank: 115
    paper_rank: 115
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (ceil(n/2)) [PNA]
    model_key: reconstr. (ceil(n/2)) [pna]
    model_plain: Reconstr. (ceil(n/2)) [PNA]
    value: 0.1233
    std: 0.012
    paper_value: 0.1233
    paper_std: 0.012
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1233
    true_std: 0.012
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1233
    sort_std: 0.012
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Reconstr. (ceil(n/2)) [GCN]
    model_key: reconstr. (ceil(n/2)) [gcn]
    model_plain: Reconstr. (ceil(n/2)) [GCN]
    value: 0.1169
    std: 0.0141
    paper_value: 0.1169
    paper_std: 0.0141
    metric: AP
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB graph classification task
    date: Oct 1, 2021
    date_display: Oct 2021
    date_iso: '2021-10-01'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-01'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1169
    true_std: 0.0141
    value_gap_source_arxiv: '2110.00577'
    value_gap_source_title: Reconstruction for Powerful Graph Representations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1169
    sort_std: 0.0141
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  rank_metric: AP
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: AP
  paper_metrics:
  - AP
  metric: AP
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
  - *id002
- benchmark: MoleculeNet
  datasets:
  - *id003
- benchmark: GNNBenchmark
  datasets:
  - *id004
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
    - dataset: ogbg-molpcba
      dataset_slug: ogbg-molpcba
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: Tox21
      dataset_slug: tox21
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CSL
      dataset_slug: csl
main_figure: /figures/2110.00577/main_figure.jpegoptim.jpg
---

