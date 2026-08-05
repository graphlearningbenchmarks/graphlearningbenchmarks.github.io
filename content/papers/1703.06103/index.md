---
title: Modeling Relational Data with Graph Convolutional Networks
arxiv_id: '1703.06103'
source_url: ''
authors:
- name: M. Schlichtkrull
  orcid: null
  s2_author_id: '8804828'
  s2_url: null
- name: Thomas Kipf
  orcid: null
  s2_author_id: '41016725'
  s2_url: null
- name: Peter Bloem
  orcid: null
  s2_author_id: '2789097'
  s2_url: null
- name: Rianne van den Berg
  orcid: null
  s2_author_id: '9965217'
  s2_url: null
- name: Ivan Titov
  orcid: null
  s2_author_id: '144889265'
  s2_url: null
- name: M. Welling
  orcid: null
  s2_author_id: '1678311'
  s2_url: null
published_date: Mar 17, 2017
published_date_iso: '2017-03-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Knowledge graphs enable a wide variety of applications, including question
  answering and information retrieval. Despite the great effort invested in their
  creation and maintenance, even the largest (e.g., Yago, DBPedia or Wikidata) remain
  incomplete. We introduce Relational Graph Convolutional Networks (R-GCNs) and apply
  them to two standard knowledge base completion tasks: Link prediction (recovery
  of missing facts, i.e. subject-predicate-object triples) and entity classification
  (recovery of missing entity attributes). R-GCNs are related to a recent class of
  neural networks operating on graphs, and are developed specifically to deal with
  the highly multi-relational data characteristic of realistic knowledge bases. We
  demonstrate the effectiveness of R-GCNs as a stand-alone model for entity classification.
  We further show that factorization models for link prediction such as DistMult can
  be significantly improved by enriching them with an encoder model to accumulate
  evidence over multiple inference steps in the relational graph, demonstrating a
  large improvement of 29.8\'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- R-GCN
mrr: 0.084
adjusted_mrr: 0.056
mrr_dataset_count: 2
benchmark_categories:
- TU Dortmund
- Knowledge Graphs
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 1
  total: 3
task_categories:
- graph_classification
- link_prediction
experiment_scopes:
- edge-level
- graph-level
results:
- &id001
  dataset: MUTAG
  rows:
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
    value: 0.991
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: supcosine
    model_plain: ECC
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: cauemo
    model_plain: ECC
    value: 0.9692
    std: 0.0136
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.06283'
    title: 'Soft causal learning for generalized molecule property prediction: An
      environment modeling perspective'
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9692
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.8088
    std: 0.0
    paper_value: 0.8088
    paper_std: 0.0
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
    feature_source_evidence: WL tree variant from Mustard library
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Entity classification on the train/test splits provided by Ristoski
      et al. 2016
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86
    at_pub_std: 0.017
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2022-05-26'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.05120000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.904
    true_std: 0.057
    value_gap_source_arxiv: '2205.13328'
    value_gap_source_title: How Powerful are $K$-hop Message Passing Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.09520000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.057
    global_rank: 141
    paper_rank: 599
    rank_delta: 458
    rank_delta_abs: 458
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Valid Optimal Assignment Kernels and Applications
      to Graph Classification
    comparison_source_arxiv: '1606.01141'
    is_best: false
    is_std_outlier: false
  - model: Feat
    model_key: feat
    model_plain: Feat
    value: 0.7794
    std: 0.0
    paper_value: 0.7794
    paper_std: 0.0
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
    feature_source_evidence: feature-based baseline
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Entity classification on the train/test splits provided by Ristoski
      et al. 2016
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-03-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7794
    true_std: 0.0
    value_gap_source_arxiv: '1703.06103'
    value_gap_source_title: Modeling Relational Data with Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7794
    sort_std: 0.0
    global_rank: 673
    paper_rank: 673
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: R-GCN
    model_key: r-gcn
    model_plain: R-GCN
    value: 0.7323
    std: 0.0048
    paper_value: 0.7323
    paper_std: 0.0048
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
    feature_source_evidence: The model uses node representations supplied by R-GCN;
      for featureless approach, it uses one-hot vectors.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Entity classification on the train/test splits provided by Ristoski
      et al. 2016
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-03-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7323
    true_std: 0.0048
    value_gap_source_arxiv: '1703.06103'
    value_gap_source_title: Modeling Relational Data with Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7323
    sort_std: 0.0048
    global_rank: 744
    paper_rank: 744
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RDF2Vec
    model_key: rdf2vec
    model_plain: RDF2Vec
    value: 0.672
    std: 0.0124
    paper_value: 0.672
    paper_std: 0.0124
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: implementation provided by the authors of Ristoski et
      al. 2016
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Entity classification on the train/test splits provided by Ristoski
      et al. 2016
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-03-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.672
    true_std: 0.0124
    value_gap_source_arxiv: '1703.06103'
    value_gap_source_title: Modeling Relational Data with Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.672
    sort_std: 0.0124
    global_rank: 774
    paper_rank: 774
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
- &id002
  dataset: WN18
  rows:
  - model: TripleRE
    model_key: rotate
    model_plain: TripleRE
    value: 0.949
    std: 0.0
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1902.10197'
    title: 'RotatE: Knowledge Graph Embedding by Relational Rotation in Complex Space'
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/DeepGraphLearning/KnowledgeGraphEmbedding
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.949
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ComplEx
    model_key: complex
    model_plain: ComplEx
    value: 0.941
    std: null
    paper_value: 0.941
    paper_std: null
    metric: MRR
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
    source_ref: complex-complex_embeddings_for_simple_link_prediction
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 link prediction task
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-03-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.941
    true_std: null
    value_gap_source_arxiv: '1703.06103'
    value_gap_source_title: Modeling Relational Data with Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.941
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
  - model: LinkFeat
    model_key: linkfeat
    model_plain: LinkFeat
    value: 0.938
    std: null
    paper_value: 0.938
    paper_std: null
    metric: MRR
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
    source_ref: toutanova2015observed
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 link prediction task
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-03-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.938
    true_std: null
    value_gap_source_arxiv: '1703.06103'
    value_gap_source_title: Modeling Relational Data with Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.938
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
  - model: HolE
    model_key: hole
    model_plain: HolE
    value: 0.938
    std: null
    paper_value: 0.938
    paper_std: null
    metric: MRR
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
    source_ref: nickel2015holographic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 link prediction task
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.938
    at_pub_std: null
    at_pub_source_arxiv: '1606.06357'
    at_pub_source_title: Complex Embeddings for Simple Link Prediction
    at_pub_source_date_iso: '2016-06-19'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2016-06-19'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.938
    true_std: null
    value_gap_source_arxiv: '1606.06357'
    value_gap_source_title: Complex Embeddings for Simple Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.938
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
  - model: DistMult
    model_key: distmult
    model_plain: DistMult
    value: 0.813
    std: null
    paper_value: 0.813
    paper_std: null
    metric: MRR
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 link prediction task
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.822
    at_pub_std: null
    at_pub_source_arxiv: '1606.06357'
    at_pub_source_title: Complex Embeddings for Simple Link Prediction
    at_pub_source_date_iso: '2016-06-19'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2016-06-19'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: 0.009000000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.822
    true_std: null
    value_gap_source_arxiv: '1606.06357'
    value_gap_source_title: Complex Embeddings for Simple Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.009000000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: null
    global_rank: 5
    paper_rank: 6
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Complex Embeddings for Simple Link Prediction
    comparison_source_arxiv: '1606.06357'
    is_best: false
    is_std_outlier: false
  - model: R-GCN
    model_key: r-gcn
    model_plain: R-GCN
    value: 0.819
    std: null
    paper_value: 0.819
    paper_std: null
    metric: MRR
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
    feature_source_evidence: R-GCN+ denotes an ensemble between R-GCN and DistMult
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 link prediction task
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-03-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.819
    true_std: null
    value_gap_source_arxiv: '1703.06103'
    value_gap_source_title: Modeling Relational Data with Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: null
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
  - model: TransE
    model_key: transe
    model_plain: TransE
    value: 0.454
    std: null
    paper_value: 0.454
    paper_std: null
    metric: MRR
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
    source_ref: bordes2013translating
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 link prediction task
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.454
    at_pub_std: null
    at_pub_source_arxiv: '1606.06357'
    at_pub_source_title: Complex Embeddings for Simple Link Prediction
    at_pub_source_date_iso: '2016-06-19'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2016-06-19'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.454
    true_std: null
    value_gap_source_arxiv: '1606.06357'
    value_gap_source_title: Complex Embeddings for Simple Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.454
    sort_std: null
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
  - model: CP
    model_key: cp
    model_plain: CP
    value: 0.058
    std: null
    paper_value: 0.058
    paper_std: null
    metric: MRR
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
    source_ref: hitchcock1927expression
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 link prediction task
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.075
    at_pub_std: null
    at_pub_source_arxiv: '1606.06357'
    at_pub_source_title: Complex Embeddings for Simple Link Prediction
    at_pub_source_date_iso: '2016-06-19'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2016-06-19'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: 0.016999999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.075
    true_std: null
    value_gap_source_arxiv: '1606.06357'
    value_gap_source_title: Complex Embeddings for Simple Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.016999999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.075
    sort_std: null
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Complex Embeddings for Simple Link Prediction
    comparison_source_arxiv: '1606.06357'
    is_best: false
    is_std_outlier: false
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
- benchmark: Knowledge Graphs
  datasets:
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: WN18
      dataset_slug: wn18
single_proposed_model: R-GCN
main_figure: /figures/1703.06103/main_figure.jpegoptim.jpg
---

