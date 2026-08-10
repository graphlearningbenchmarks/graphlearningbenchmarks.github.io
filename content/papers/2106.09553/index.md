---
title: How Much Structural Information Large Scale Molecular Language Representations
  Can Capture?
arxiv_id: '2106.09553'
source_url: ''
authors:
- name: Jerret Ross
  orcid: null
  s2_author_id: '39320489'
  s2_url: null
- name: Brian Belgodere
  orcid: null
  s2_author_id: '2679155'
  s2_url: null
- name: Vijil Chenthamarakshan
  orcid: null
  s2_author_id: '46542047'
  s2_url: null
- name: Inkit Padhi
  orcid: null
  s2_author_id: '8350409'
  s2_url: null
- name: Youssef Mroueh
  orcid: null
  s2_author_id: '2211263'
  s2_url: null
- name: Payel Das
  orcid: null
  s2_author_id: '1730372'
  s2_url: null
published_date: Jun 17, 2021
published_date_iso: '2021-06-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Predicting the properties of a chemical molecule is of great importance
  in many applications, including drug discovery and material design. Machine learning-based
  models promise to enable more accurate and faster molecular property predictions
  than the current state-of-the-art techniques, such as Density Functional Theory
  calculations or wet-lab experiments. Various supervised machine learning models,
  including graph neural nets, have demonstrated promising performance in molecular
  property prediction tasks. However, the vast chemical space and the limited availability
  of property labels make supervised learning challenging, calling for learning a
  general-purpose molecular representation. Recently, unsupervised transformer-based
  language models pre-trained on large unlabeled corpus have produced state-of-the-art
  results in many downstream natural language processing tasks. Inspired by this development,
  we present molecular embeddings obtained by training an efficient transformer encoder
  model, MoLFormer, which uses rotary positional embeddings. This model employs a
  linear attention mechanism, coupled with highly distributed training, on SMILES
  sequences of 1.1 billion unlabeled molecules from the PubChem and ZINC datasets.
  Experiments show that utilizing the learned molecular representation outperforms
  existing baselines on downstream tasks, including supervised and self-supervised
  graph neural net baselines and language models, on several classification and regression
  tasks from ten benchmark datasets while performing competitively on two others.
  Further analyses, specifically through the lens of attention, demonstrate that MoLFormer
  trained on chemical SMILES indeed learns the spatial relationships between atoms
  within a molecule. These results provide encouraging evidence that the large-scale
  molecular language models can capture sufficient chemical and structural information
  to predict various distinct molecular properties, including quantum-chemical properties.
codebase_url: https://github.com/IBM/molformer
extraction_model: google/gemma-4-31B-it
has_results: true
paper_type: method
proposed_models:
- MoLFormer-XL
- MoLFormer-Base
mrr: 0.1562
adjusted_mrr: 0.1042
mrr_dataset_count: 2
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 2
  total: 9
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: BACE
  rows:
  - model: ProtoMol
    model_key: protomol
    model_plain: ProtoMol
    value: 0.914
    std: 0.003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.16824'
    title: 'ProtoMol: Enhancing Molecular Property Prediction via Prototype-Guided
      Multimodal Learning'
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    venue: Briefings Bioinform.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.914
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MMSG
    model_key: mmsg
    model_plain: MMSG
    value: 0.908
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
    arxiv_id: '2510.16824'
    title: 'ProtoMol: Enhancing Molecular Property Prediction via Prototype-Guided
      Multimodal Learning'
    date: Oct 19, 2025
    date_display: Oct 2025
    date_iso: '2025-10-19'
    venue: Briefings Bioinform.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.908
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.907
    std: 0.0
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.907
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolCLR
    model_key: molclr
    model_plain: MolCLR
    value: 0.89
    std: null
    paper_value: 0.89
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: self-supervised learning framework based on GIN
    table_ref: Table 1
    source_ref: wang2021molclr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.89
    true_std: 0.003
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.89
    sort_std: 0.003
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
  - model: MoLFormer-XL
    model_key: molformer-xl
    model_plain: MoLFormer-XL
    value: 0.8821
    std: null
    paper_value: 0.8821
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: trained on a large corpus of 1.1 billion molecules
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-17'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8821
    true_std: null
    value_gap_source_arxiv: '2106.09553'
    value_gap_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8821
    sort_std: null
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D-MPNN
    model_key: d-mpnn
    model_plain: D-MPNN
    value: 0.853
    std: null
    paper_value: 0.853
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: doi:10.1021/acs.jcim.9b00237
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.865
    at_pub_std: 0.013
    at_pub_source_arxiv: '2006.04804'
    at_pub_source_title: Optimal Transport Graph Neural Networks
    at_pub_source_date_iso: '2020-06-08'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.01200000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.878
    true_std: 0.032
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.025000000000000022
    has_value_note: false
    value_note: ''
    sort_value: 0.878
    sort_std: 0.032
    global_rank: 20
    paper_rank: 66
    rank_delta: 46
    rank_delta_abs: 46
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: N-GRAM
    model_key: n-gram
    model_plain: N-GRAM
    value: 0.876
    std: null
    paper_value: 0.876
    paper_std: null
    metric: ROC-AUC
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
    feature_source_evidence: embedding the nodes in a graph and then constructing
      a compact representation of the graph by assembling the vertex embeddings in
      short walks
    table_ref: Table 1
    source_ref: liu2019ngram
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.876
    true_std: 0.035
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.876
    sort_std: 0.035
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
  - model: rf
    model_key: rf
    model_plain: rf
    value: 0.867
    std: null
    paper_value: 0.867
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: shallow machine learning models trained on molecular
      fingerprints
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-17'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.867
    true_std: null
    value_gap_source_arxiv: '2106.09553'
    value_gap_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.867
    sort_std: null
    global_rank: 39
    paper_rank: 39
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
    value: 0.8646
    std: 0.0081
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.15589'
    title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
      Graph Information Bottleneck
    date: Dec 20, 2024
    date_display: Dec 2024
    date_iso: '2024-12-20'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/NSLab-CUK/S-CGIB
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 43
    sort_value: 0.8646
    sort_std: 0.0081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SVM
    model_key: svm
    model_plain: SVM
    value: 0.862
    std: null
    paper_value: 0.862
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: shallow machine learning models trained on molecular
      fingerprints
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-17'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.862
    true_std: null
    value_gap_source_arxiv: '2106.09553'
    value_gap_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.862
    sort_std: null
    global_rank: 49
    paper_rank: 49
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Hu, et al.
    model_key: hu, et al.
    model_plain: Hu, et al.
    value: 0.859
    std: null
    paper_value: 0.859
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: pre-trains a Graph Isomorphism Network (GIN) on molecular
      graphs
    table_ref: Table 1
    source_ref: hu2020strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-17'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.859
    true_std: null
    value_gap_source_arxiv: '2106.09553'
    value_gap_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.859
    sort_std: null
    global_rank: 56
    paper_rank: 56
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.856
    std: null
    paper_value: 0.856
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: geometry-aware GNN baselines
    table_ref: Table 1
    source_ref: fang2022geometry
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.856
    true_std: 0.011
    value_gap_source_arxiv: '2605.06462'
    value_gap_source_title: Invariant-Based Diagnostics for Graph Benchmarks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.856
    sort_std: 0.011
    global_rank: 62
    paper_rank: 62
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoLFormer-Base
    model_key: molformer-base
    model_plain: MoLFormer-Base
    value: 0.828
    std: null
    paper_value: 0.828
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: pre-trained on smaller datasets
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-17'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.828
    true_std: null
    value_gap_source_arxiv: '2106.09553'
    value_gap_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.828
    sort_std: null
    global_rank: 113
    paper_rank: 113
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMVP-C
    model_key: graphmvp-c
    model_plain: GraphMVP-C
    value: 0.812
    std: null
    paper_value: 0.812
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: self-supervised learning (SSL) is performed by leveraging
      the correspondence and consistency between 2D topological structures and 3D
      geometric views
    table_ref: Table 1
    source_ref: liu2021pre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.812
    true_std: 0.009
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.812
    sort_std: 0.009
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
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.734
    std: null
    paper_value: 0.734
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: DBLP:conf/aaai/Lu0WHLH19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: BACE classification benchmark using MoleculeNet scaffold data splits,
      ROC-AUC metric
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.734
    true_std: 0.03
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.734
    sort_std: 0.03
    global_rank: 261
    paper_rank: 261
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
  dataset: BBBP
  rows:
  - model: MAGPrompt+
    model_key: magprompt+
    model_plain: MAGPrompt+
    value: 0.9432
    std: 0.0238
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.05567'
    title: 'MAGPrompt: Message-Adaptive Graph Prompt Tuning for Graph Neural Networks'
    date: Feb 5, 2026
    date_display: Feb 2026
    date_iso: '2026-02-05'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9432
    sort_std: 0.0238
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CamS-LLaMA
    model_key: cams-llama
    model_plain: CamS-LLaMA
    value: 0.942
    std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 100.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2601.02530'
    title: 'Multi-scale Graph Autoregressive Modeling: Molecular Property Prediction
      via Next Token Prediction'
    date: Jan 5, 2026
    date_display: Jan 2026
    date_iso: '2026-01-05'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.942
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SE(3)-I MPPH
    model_key: se(3)-i mpph
    model_plain: SE(3)-I MPPH
    value: 0.94
    std: 0.021
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
    global_rank: 3
    sort_value: 0.94
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MoLFormer-XL
    model_key: molformer-xl
    model_plain: MoLFormer-XL
    value: 0.937
    std: null
    paper_value: 0.937
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: trained on a large corpus of 1.1 billion molecules
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-17'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.937
    true_std: null
    value_gap_source_arxiv: '2106.09553'
    value_gap_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.937
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
    is_best: true
    is_std_outlier: false
  - model: D-MPNN
    model_key: d-mpnn
    model_plain: D-MPNN
    value: 0.712
    std: null
    paper_value: 0.712
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: doi:10.1021/acs.jcim.9b00237
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.708
    at_pub_std: null
    at_pub_source_arxiv: '2010.09885'
    at_pub_source_title: 'ChemBERTa: Large-Scale Self-Supervised Pretraining for Molecular
      Property Prediction'
    at_pub_source_date_iso: '2020-10-19'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.913
    true_std: 0.026
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.20100000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.913
    sort_std: 0.026
    global_rank: 26
    paper_rank: 117
    rank_delta: 91
    rank_delta_abs: 91
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'ChemBERTa: Large-Scale Self-Supervised Pretraining for
      Molecular Property Prediction'
    comparison_source_arxiv: '2010.09885'
    is_best: true
    is_std_outlier: false
  - model: N-GRAM
    model_key: n-gram
    model_plain: N-GRAM
    value: 0.912
    std: null
    paper_value: 0.912
    paper_std: null
    metric: ROC-AUC
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
    feature_source_evidence: embedding the nodes in a graph and then constructing
      a compact representation of the graph by assembling the vertex embeddings in
      short walks
    table_ref: Table 1
    source_ref: liu2019ngram
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.912
    true_std: 0.03
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.912
    sort_std: 0.03
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MoLFormer-Base
    model_key: molformer-base
    model_plain: MoLFormer-Base
    value: 0.909
    std: null
    paper_value: 0.909
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: pre-trained on large unlabeled corpora
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-17'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.909
    true_std: null
    value_gap_source_arxiv: '2106.09553'
    value_gap_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.909
    sort_std: null
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8875
    std: 0.0049
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.15589'
    title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
      Graph Information Bottleneck
    date: Dec 20, 2024
    date_display: Dec 2024
    date_iso: '2024-12-20'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/NSLab-CUK/S-CGIB
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 34
    sort_value: 0.8875
    sort_std: 0.0049
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.85
    std: null
    paper_value: 0.85
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: DBLP:conf/aaai/Lu0WHLH19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.85
    true_std: 0.064
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.85
    sort_std: 0.064
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
  - model: MolCLR
    model_key: molclr
    model_plain: MolCLR
    value: 0.736
    std: null
    paper_value: 0.736
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: self-supervised learning framework based on GIN
    table_ref: Table 1
    source_ref: wang2021molclr
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-18'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.736
    true_std: 0.005
    value_gap_source_arxiv: '2202.09346'
    value_gap_source_title: Improving Molecular Contrastive Learning via Faulty Negative
      Mitigation and Decomposed Fragment Contrast
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.736
    sort_std: 0.005
    global_rank: 78
    paper_rank: 78
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SVM
    model_key: svm
    model_plain: SVM
    value: 0.729
    std: null
    paper_value: 0.729
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: shallow machine learning models trained on molecular
      fingerprints
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.723
    at_pub_std: 0.0
    at_pub_source_arxiv: '2002.08264'
    at_pub_source_title: Molecule Attention Transformer
    at_pub_source_date_iso: '2020-02-19'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2021-06-17'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.729
    true_std: null
    value_gap_source_arxiv: '2106.09553'
    value_gap_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: null
    global_rank: 84
    paper_rank: 84
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Molecule Attention Transformer
    comparison_source_arxiv: '2002.08264'
    is_best: false
    is_std_outlier: false
  - model: rf
    model_key: rf
    model_plain: rf
    value: 0.714
    std: null
    paper_value: 0.714
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: shallow machine learning models trained on molecular
      fingerprints
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.725
    at_pub_std: 0.006
    at_pub_source_arxiv: '2002.08264'
    at_pub_source_title: Molecule Attention Transformer
    at_pub_source_date_iso: '2020-02-19'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-02-19'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.01100000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.725
    true_std: 0.006
    value_gap_source_arxiv: '2002.08264'
    value_gap_source_title: Molecule Attention Transformer
    value_gap_source_is_current_paper: false
    value_gap: 0.01100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.725
    sort_std: 0.006
    global_rank: 91
    paper_rank: 116
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecule Attention Transformer
    comparison_source_arxiv: '2002.08264'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP-C
    model_key: graphmvp-c
    model_plain: GraphMVP-C
    value: 0.724
    std: null
    paper_value: 0.724
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: self-supervised learning (SSL) is performed by leveraging
      the correspondence and consistency between 2D topological structures and 3D
      geometric views
    table_ref: Table 1
    source_ref: liu2021pre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.724
    true_std: 0.016
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.724
    sort_std: 0.016
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
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.724
    std: null
    paper_value: 0.724
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: fang2022geometry
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.724
    true_std: 0.004
    value_gap_source_arxiv: '2605.06462'
    value_gap_source_title: Invariant-Based Diagnostics for Graph Benchmarks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.724
    sort_std: 0.004
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
  - model: Hu, et al.
    model_key: hu, et al.
    model_plain: Hu, et al.
    value: 0.708
    std: null
    paper_value: 0.708
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: pre-trains a Graph Isomorphism Network (GIN...)
    table_ref: Table 1
    source_ref: hu2020strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-17'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.708
    true_std: null
    value_gap_source_arxiv: '2106.09553'
    value_gap_source_title: How Much Structural Information Large Scale Molecular
      Language Representations Can Capture?
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.708
    sort_std: null
    global_rank: 126
    paper_rank: 126
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChemBERTa
    model_key: chemberta
    model_plain: ChemBERTa
    value: 0.643
    std: null
    paper_value: 0.643
    paper_std: null
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
    input_feature_source: llm_features
    feature_source_evidence: pre-trained molecular language model trained on a smaller
      chemical dataset
    table_ref: Table 1
    source_ref: chithrananda2020chemberta
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BBBP using MoleculeNet scaffold data splits
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-22'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.643
    true_std: null
    value_gap_source_arxiv: '2310.14216'
    value_gap_source_title: 'UniMAP: Universal SMILES-Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.643
    sort_std: null
    global_rank: 284
    paper_rank: 284
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
- benchmark: MoleculeNet
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: BACE
      dataset_slug: bace
    - dataset: BBBP
      dataset_slug: bbbp
main_figure: /figures/2106.09553/main_figure.jpegoptim.jpg
---

