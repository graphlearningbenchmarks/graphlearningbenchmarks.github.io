---
title: Molecular Topological Profile (MOLTOP) - Simple and Strong Baseline for Molecular
  Graph Classification
arxiv_id: '2407.12136'
source_url: ''
authors:
- name: Jakub Adamczyk
  orcid: null
  s2_author_id: '2311887144'
  s2_url: null
- name: Wojciech Czech
  orcid: null
  s2_author_id: '2311699477'
  s2_url: null
published_date: Jul 16, 2024
published_date_iso: '2024-07-16'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: We revisit the effectiveness of topological descriptors for molecular graph
  classification and design a simple, yet strong baseline. We demonstrate that a simple
  approach to feature engineering - employing histogram aggregation of edge descriptors
  and one-hot encoding for atomic numbers and bond types - when combined with a Random
  Forest classifier, can establish a strong baseline for Graph Neural Networks (GNNs).
  The novel algorithm, Molecular Topological Profile (MOLTOP), integrates Edge Betweenness
  Centrality, Adjusted Rand Index and SCAN Structural Similarity score. This approach
  proves to be remarkably competitive when compared to modern GNNs, while also being
  simple, fast, low-variance and hyperparameter-free. Our approach is rigorously tested
  on MoleculeNet datasets using fair evaluation protocol provided by Open Graph Benchmark.
  We additionally show out-of-domain generation capabilities on peptide classification
  task from Long Range Graph Benchmark. The evaluations across eleven benchmark datasets
  reveal MOLTOP's strong discriminative capabilities, surpassing the $1$-WL test and
  even $3$-WL test for some classes of graphs. Our conclusion is that descriptor-based
  baselines, such as the one we propose, are still crucial for accurately assessing
  advancements in the GNN domain.
codebase_url: https://github.com/j-adamczyk/MOLTOP
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MOLTOP
mrr: 0.0078
adjusted_mrr: 0.0078
mrr_dataset_count: 4
benchmark_categories:
- MoleculeNet
- LRGB
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 3
  total: 9
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 1
  total: 5
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: BACE
  rows:
  - model: MAGPrompt+
    model_key: protomol
    model_plain: MAGPrompt+
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
  - model: MAGPrompt+
    model_key: mmsg
    model_plain: MAGPrompt+
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
  - model: MAGPrompt+
    model_key: memgnn
    model_plain: MAGPrompt+
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
  - model: D-MPNN
    model_key: d-mpnn
    model_plain: D-MPNN
    value: 0.809
    std: 0.006
    paper_value: 0.809
    paper_std: 0.006
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.878
    at_pub_std: 0.032
    at_pub_source_arxiv: '2312.07633'
    at_pub_source_title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    at_pub_source_date_iso: '2023-12-12'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.06899999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.878
    true_std: 0.032
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.06899999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.878
    sort_std: 0.032
    global_rank: 19
    paper_rank: 154
    rank_delta: 135
    rank_delta_abs: 135
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    comparison_source_arxiv: '2312.07633'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.845
    std: 0.007
    paper_value: 0.845
    paper_std: 0.007
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.861
    at_pub_std: 0.013
    at_pub_source_arxiv: '2006.04804'
    at_pub_source_title: Optimal Transport Graph Neural Networks
    at_pub_source_date_iso: '2020-06-08'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8646
    true_std: 0.0081
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.019600000000000062
    has_value_note: false
    value_note: ''
    sort_value: 0.8646
    sort_std: 0.0081
    global_rank: 41
    paper_rank: 78
    rank_delta: 37
    rank_delta_abs: 37
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AttentiveFP
    model_key: attentivefp
    model_plain: AttentiveFP
    value: 0.784
    std: 0.022
    paper_value: 0.784
    paper_std: 0.022
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.863
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.07899999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.863
    true_std: null
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.07899999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.863
    sort_std: null
    global_rank: 43
    paper_rank: 203
    rank_delta: 160
    rank_delta_abs: 160
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    comparison_source_arxiv: '2110.01191'
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.856
    std: 0.011
    paper_value: 0.856
    paper_std: 0.011
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
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
    value_gap_source_arxiv: '2604.16586'
    value_gap_source_title: A Systematic Survey and Benchmark of Deep Learning for
      Molecular Property Prediction in the Foundation Model Era
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.856
    sort_std: 0.011
    global_rank: 58
    paper_rank: 58
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
    value: 0.823
    std: 0.034
    paper_value: 0.823
    paper_std: 0.034
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.854
    at_pub_std: 0.011
    at_pub_source_arxiv: '2310.07351'
    at_pub_source_title: Atom-Motif Contrastive Transformer for Molecular Property
      Prediction
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.031000000000000028
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.854
    true_std: 0.011
    value_gap_source_arxiv: '2310.07351'
    value_gap_source_title: Atom-Motif Contrastive Transformer for Molecular Property
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.031000000000000028
    has_value_note: false
    value_note: ''
    sort_value: 0.854
    sort_std: 0.011
    global_rank: 60
    paper_rank: 117
    rank_delta: 57
    rank_delta_abs: 57
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.807
    std: 0.009
    paper_value: 0.807
    paper_std: 0.009
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8451
    at_pub_std: null
    at_pub_source_arxiv: '2211.03666'
    at_pub_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    at_pub_source_date_iso: '2022-11-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.03809999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8451
    true_std: null
    value_gap_source_arxiv: '2211.03666'
    value_gap_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    value_gap_source_is_current_paper: false
    value_gap: 0.03809999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.8451
    sort_std: null
    global_rank: 78
    paper_rank: 156
    rank_delta: 78
    rank_delta_abs: 78
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    comparison_source_arxiv: '2211.03666'
    is_best: false
    is_std_outlier: false
  - model: ECFP
    model_key: ecfp
    model_plain: ECFP
    value: 0.838
    std: 0.004
    paper_value: 0.838
    paper_std: 0.004
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.838
    true_std: 0.004
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.838
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
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.729
    std: 0.02
    paper_value: 0.729
    paper_std: 0.02
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.834
    at_pub_std: 0.033
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.10499999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.834
    true_std: 0.033
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.10499999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.834
    sort_std: 0.033
    global_rank: 97
    paper_rank: 252
    rank_delta: 155
    rank_delta_abs: 155
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: MOLTOP
    model_key: moltop
    model_plain: MOLTOP
    value: 0.829
    std: 0.002
    paper_value: 0.829
    paper_std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: mixed
    feature_source_evidence: utilizing both topological descriptors and simple atom
      and bond features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.829
    true_std: 0.002
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: 0.002
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
  - model: GROVER
    model_key: grover
    model_plain: GROVER
    value: 0.81
    std: 0.014
    paper_value: 0.81
    paper_std: 0.014
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.826
    at_pub_std: 0.007
    at_pub_source_arxiv: '2405.10343'
    at_pub_source_title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view
      Molecular Representation Learning'
    at_pub_source_date_iso: '2024-05-15'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-05-15'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.015999999999999903
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.826
    true_std: 0.007
    value_gap_source_arxiv: '2405.10343'
    value_gap_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.015999999999999903
    has_value_note: false
    value_note: ''
    sort_value: 0.826
    sort_std: 0.007
    global_rank: 112
    paper_rank: 148
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.768
    std: 0.011
    paper_value: 0.768
    paper_std: 0.011
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.812
    at_pub_std: 0.009
    at_pub_source_arxiv: '2207.08806'
    at_pub_source_title: Unified 2D and 3D Pre-Training of Molecular Representations
    at_pub_source_date_iso: '2022-07-14'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-04-17'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.04400000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.812
    true_std: null
    value_gap_source_arxiv: '2404.11568'
    value_gap_source_title: On the Scalability of GNNs for Molecular Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.04400000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.812
    sort_std: null
    global_rank: 141
    paper_rank: 224
    rank_delta: 83
    rank_delta_abs: 83
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unified 2D and 3D Pre-Training of Molecular Representations
    comparison_source_arxiv: '2207.08806'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP-C
    model_key: graphmvp-c
    model_plain: GraphMVP-C
    value: 0.812
    std: 0.009
    paper_value: 0.812
    paper_std: 0.009
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
    input_feature_source: raw_features
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.812
    at_pub_std: 0.009
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
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
    value_gap_source_arxiv: '2110.07728'
    value_gap_source_title: 16 Pre-training Molecular Graph Representation with 3D
      Geometry
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.812
    sort_std: 0.009
    global_rank: 142
    paper_rank: 142
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LTP
    model_key: ltp
    model_plain: LTP
    value: 0.807
    std: 0.003
    paper_value: 0.807
    paper_std: 0.003
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.807
    true_std: 0.003
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.807
    sort_std: 0.003
    global_rank: 158
    paper_rank: 158
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LDP
    model_key: ldp
    model_plain: LDP
    value: 0.805
    std: 0.003
    paper_value: 0.805
    paper_std: 0.003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8016
    at_pub_std: null
    at_pub_source_arxiv: '2211.03666'
    at_pub_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    at_pub_source_date_iso: '2022-11-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0034000000000000696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.805
    true_std: 0.003
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.805
    sort_std: 0.003
    global_rank: 161
    paper_rank: 161
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    comparison_source_arxiv: '2211.03666'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.687
    std: 0.078
    paper_value: 0.687
    paper_std: 0.078
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.782
    at_pub_std: 0.012
    at_pub_source_arxiv: '2205.15746'
    at_pub_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    at_pub_source_date_iso: '2022-05-31'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.09499999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.782
    true_std: 0.012
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.09499999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.012
    global_rank: 205
    paper_rank: 278
    rank_delta: 73
    rank_delta_abs: 73
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    comparison_source_arxiv: '2205.15746'
    is_best: false
    is_std_outlier: false
  - model: molecular fingerprint
    model_key: molecular fingerprint
    model_plain: molecular fingerprint
    value: 0.715
    std: 0.002
    paper_value: 0.715
    paper_std: 0.002
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.715
    true_std: 0.002
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.715
    sort_std: 0.002
    global_rank: 265
    paper_rank: 265
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
  - model: MAGPrompt+
    model_key: cams-llama
    model_plain: MAGPrompt+
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
  - model: MAGPrompt+
    model_key: se(3)-i mpph
    model_plain: MAGPrompt+
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.687
    std: 0.013
    paper_value: 0.687
    paper_std: 0.013
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.873
    at_pub_std: 0.036
    at_pub_source_arxiv: '2208.04529'
    at_pub_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    at_pub_source_date_iso: '2022-08-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.18599999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8875
    true_std: 0.0049
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.2004999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8875
    sort_std: 0.0049
    global_rank: 32
    paper_rank: 177
    rank_delta: 145
    rank_delta_abs: 145
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    comparison_source_arxiv: '2208.04529'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.675
    std: 0.033
    paper_value: 0.675
    paper_std: 0.033
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.887
    at_pub_std: 0.019
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.21199999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.887
    true_std: 0.019
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.21199999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.887
    sort_std: 0.019
    global_rank: 34
    paper_rank: 209
    rank_delta: 175
    rank_delta_abs: 175
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: GROVER
    model_key: grover
    model_plain: GROVER
    value: 0.695
    std: 0.001
    paper_value: 0.695
    paper_std: 0.001
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.887
    at_pub_std: 0.006
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.19200000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.887
    true_std: 0.006
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.19200000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.887
    sort_std: 0.006
    global_rank: 35
    paper_rank: 159
    rank_delta: 124
    rank_delta_abs: 124
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.706
    std: 0.016
    paper_value: 0.706
    paper_std: 0.016
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.881
    at_pub_std: 0.036
    at_pub_source_arxiv: '2208.04529'
    at_pub_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    at_pub_source_date_iso: '2022-08-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-08-09'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.17500000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.881
    true_std: 0.036
    value_gap_source_arxiv: '2208.04529'
    value_gap_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    value_gap_source_is_current_paper: false
    value_gap: 0.17500000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.881
    sort_std: 0.036
    global_rank: 36
    paper_rank: 119
    rank_delta: 83
    rank_delta_abs: 83
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    comparison_source_arxiv: '2208.04529'
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.66
    std: 0.006
    paper_value: 0.66
    paper_std: 0.006
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.879
    at_pub_std: 0.02
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.21899999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.879
    true_std: 0.02
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.21899999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.879
    sort_std: 0.02
    global_rank: 37
    paper_rank: 243
    rank_delta: 206
    rank_delta_abs: 206
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.685
    std: 0.002
    paper_value: 0.685
    paper_std: 0.002
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86
    at_pub_std: 0.034
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.17499999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.86
    true_std: 0.034
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.17499999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.034
    global_rank: 47
    paper_rank: 181
    rank_delta: 134
    rank_delta_abs: 134
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.696
    std: 0.019
    paper_value: 0.696
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.645
    at_pub_std: 0.031
    at_pub_source_arxiv: '2209.15101'
    at_pub_source_title: Improving Molecular Pretraining with Complementary Featurizations
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.050999999999999934
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8304
    true_std: 0.0038
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.13440000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8304
    sort_std: 0.0038
    global_rank: 55
    paper_rank: 157
    rank_delta: 102
    rank_delta_abs: 102
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Improving Molecular Pretraining with Complementary Featurizations
    comparison_source_arxiv: '2209.15101'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP-C
    model_key: graphmvp-c
    model_plain: GraphMVP-C
    value: 0.724
    std: 0.016
    paper_value: 0.724
    paper_std: 0.016
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
    input_feature_source: raw_features
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.724
    at_pub_std: 0.016
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
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
    value_gap_source_arxiv: '2110.07728'
    value_gap_source_title: 16 Pre-training Molecular Graph Representation with 3D
      Geometry
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.724
    sort_std: 0.016
    global_rank: 87
    paper_rank: 87
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
    std: 0.004
    paper_value: 0.724
    paper_std: 0.004
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
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
    value_gap_source_arxiv: '2604.16586'
    value_gap_source_title: A Systematic Survey and Benchmark of Deep Learning for
      Molecular Property Prediction in the Foundation Model Era
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.724
    sort_std: 0.004
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
  - model: MOLTOP
    model_key: moltop
    model_plain: MOLTOP
    value: 0.689
    std: 0.002
    paper_value: 0.689
    paper_std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: mixed
    feature_source_evidence: utilizing both topological descriptors and simple atom
      and bond features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.689
    true_std: 0.002
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.689
    sort_std: 0.002
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
  - model: ECFP
    model_key: ecfp
    model_plain: ECFP
    value: 0.686
    std: 0.005
    paper_value: 0.686
    paper_std: 0.005
    metric: ROC-AUC
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
    feature_source_evidence: molecular fingerprint
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.686
    true_std: 0.005
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.686
    sort_std: 0.005
    global_rank: 180
    paper_rank: 180
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Adding atoms and bonds features
    model_key: adding atoms and bonds features
    model_plain: Adding atoms and bonds features
    value: 0.684
    std: 0.006
    paper_value: 0.684
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
    input_feature_source: mixed
    feature_source_evidence: Adding atoms and bonds features
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.684
    true_std: 0.006
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.684
    sort_std: 0.006
    global_rank: 185
    paper_rank: 185
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LTP
    model_key: ltp
    model_plain: LTP
    value: 0.656
    std: 0.003
    paper_value: 0.656
    paper_std: 0.003
    metric: ROC-AUC
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
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.656
    true_std: 0.003
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.656
    sort_std: 0.003
    global_rank: 253
    paper_rank: 253
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Adding topological edge features
    model_key: adding topological edge features
    model_plain: Adding topological edge features
    value: 0.65
    std: 0.005
    paper_value: 0.65
    paper_std: 0.005
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
    input_feature_source: mixed
    feature_source_evidence: Adding topological edge features
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.65
    true_std: 0.005
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.65
    sort_std: 0.005
    global_rank: 264
    paper_rank: 264
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LDP
    model_key: ldp
    model_plain: LDP
    value: 0.633
    std: 0.004
    paper_value: 0.633
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6277
    at_pub_std: null
    at_pub_source_arxiv: '2211.03666'
    at_pub_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    at_pub_source_date_iso: '2022-11-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.005299999999999971
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.633
    true_std: 0.004
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.633
    sort_std: 0.004
    global_rank: 280
    paper_rank: 280
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Application of Graph Neural Networks and graph descriptors
      for graph classification
    comparison_source_arxiv: '2211.03666'
    is_best: false
    is_std_outlier: false
  - model: LDP, 50 bins
    model_key: ldp, 50 bins
    model_plain: LDP, 50 bins
    value: 0.633
    std: 0.004
    paper_value: 0.633
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.633
    true_std: 0.004
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.633
    sort_std: 0.004
    global_rank: 281
    paper_rank: 281
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
- &id004
  dataset: Peptides-func
  rows:
  - model: Tango_GPS
    model_key: s^2gcn
    model_plain: Tango_GPS
    value: 0.7311
    std: 0.0066
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_display: Nov 2024
    date_iso: '2024-11-19'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7311
    sort_std: 0.0066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: s^2 gcn + pe
    model_plain: Tango_GPS
    value: 0.7311
    std: 0.0066
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.19121'
    title: Spatio-Spectral Graph Neural Networks
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: PE is described as stable positional encodings almost
      free of cost for S2GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.7311
    sort_std: 0.0066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: s4g
    model_plain: Tango_GPS
    value: 0.7293
    std: 0.0004
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_display: Feb 2024
    date_iso: '2024-02-13'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7293
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.593
    std: 0.0023
    paper_value: 0.593
    paper_std: 0.0023
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on peptides-func
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.686
    at_pub_std: 0.005
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.09300000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7261
    true_std: 0.0011
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.1331
    has_value_note: false
    value_note: ''
    sort_value: 0.7261
    sort_std: 0.0011
    global_rank: 5
    paper_rank: 156
    rank_delta: 151
    rank_delta_abs: 151
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph
      Benchmark
    comparison_source_arxiv: '2309.00367'
    is_best: true
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.5864
    std: 0.0077
    paper_value: 0.5864
    paper_std: 0.0077
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on peptides-func
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6765
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.09009999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7006
    true_std: 0.0033
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.11419999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7006
    sort_std: 0.0033
    global_rank: 40
    paper_rank: 163
    rank_delta: 123
    rank_delta_abs: 123
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph
      Benchmark
    comparison_source_arxiv: '2309.00367'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.5543
    std: 0.0078
    paper_value: 0.5543
    paper_std: 0.0078
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on peptides-func
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5543
    at_pub_std: 0.0078
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-04-27'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.699
    true_std: 0.003
    value_gap_source_arxiv: '2604.24293'
    value_gap_source_title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature
      Evolution via Continuous Phase Transitions'
    value_gap_source_is_current_paper: false
    value_gap: 0.14469999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.699
    sort_std: 0.003
    global_rank: 41
    paper_rank: 174
    rank_delta: 133
    rank_delta_abs: 133
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN+RWSE
    model_key: gatedgcn+rwse
    model_plain: GatedGCN+RWSE
    value: 0.6069
    std: 0.0035
    paper_value: 0.6069
    paper_std: 0.0035
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
    input_feature_source: raw_features
    feature_source_evidence: RWSE positional encodings computed on the same graph
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on peptides-func
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6685
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2301.11956'
    at_pub_source_title: On the Connection Between MPNN and Graph Transformer
    at_pub_source_date_iso: '2023-01-27'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-01-27'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.06159999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6685
    true_std: 0.0062
    value_gap_source_arxiv: '2301.11956'
    value_gap_source_title: On the Connection Between MPNN and Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: 0.06159999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.6685
    sort_std: 0.0062
    global_rank: 87
    paper_rank: 148
    rank_delta: 61
    rank_delta_abs: 61
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Connection Between MPNN and Graph Transformer
    comparison_source_arxiv: '2301.11956'
    is_best: false
    is_std_outlier: false
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.5498
    std: 0.0079
    paper_value: 0.5498
    paper_std: 0.0079
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on peptides-func
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6621
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.11230000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6621
    true_std: 0.0067
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.11230000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.6621
    sort_std: 0.0067
    global_rank: 92
    paper_rank: 177
    rank_delta: 85
    rank_delta_abs: 85
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph
      Benchmark
    comparison_source_arxiv: '2309.00367'
    is_best: false
    is_std_outlier: false
  - model: SAN+RWSE
    model_key: san+rwse
    model_plain: SAN+RWSE
    value: 0.6439
    std: 0.0075
    paper_value: 0.6439
    paper_std: 0.0075
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: RWSE positional encodings computed on the same graph
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on peptides-func
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6562
    at_pub_std: 0.0075
    at_pub_source_arxiv: '2302.08647'
    at_pub_source_title: Multiresolution Graph Transformers and Wavelet Positional
      Encoding for Learning Hierarchical Structures
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-02-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.012299999999999978
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6562
    true_std: 0.0075
    value_gap_source_arxiv: '2302.08647'
    value_gap_source_title: Multiresolution Graph Transformers and Wavelet Positional
      Encoding for Learning Hierarchical Structures
    value_gap_source_is_current_paper: false
    value_gap: 0.012299999999999978
    has_value_note: false
    value_note: ''
    sort_value: 0.6562
    sort_std: 0.0075
    global_rank: 102
    paper_rank: 125
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MOLTOP
    model_key: moltop
    model_plain: MOLTOP
    value: 0.6459
    std: 0.0005
    paper_value: 0.6459
    paper_std: 0.0005
    metric: AP
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: utilize both topological and molecular features
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on peptides-func
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.6459
    true_std: 0.0005
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6459
    sort_std: 0.0005
    global_rank: 123
    paper_rank: 123
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAN+LapPE
    model_key: san+lappe
    model_plain: SAN+LapPE
    value: 0.6384
    std: 0.0121
    paper_value: 0.6384
    paper_std: 0.0121
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: LapPE positional encodings computed on the same graph
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on peptides-func
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6384
    at_pub_std: 0.0121
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6384
    true_std: 0.0121
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6384
    sort_std: 0.0121
    global_rank: 131
    paper_rank: 131
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Transformer+LapPE
    model_key: transformer+lappe
    model_plain: Transformer+LapPE
    value: 0.6326
    std: 0.0126
    paper_value: 0.6326
    paper_std: 0.0126
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: LapPE positional encodings computed on the same graph
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on peptides-func
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6326
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6326
    true_std: 0.0126
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6326
    sort_std: 0.0126
    global_rank: 133
    paper_rank: 133
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AP
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: AP
  paper_metrics:
  - AP
  metric: AP
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: ToxCast
  rows:
  - model: GIN (Supervised EdgePred)
    model_key: geomgcl
    model_plain: GIN (Supervised EdgePred)
    value: 0.763
    std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_display: Sep 2021
    date_iso: '2021-09-24'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: The model uses 2D and 3D views derived from the molecule,
      which are standard geometric augmentations/views for this task.
    is_global_top: true
    global_rank: 1
    sort_value: 0.763
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN (Supervised EdgePred)
    model_key: light deepgpt
    model_plain: GIN (Supervised EdgePred)
    value: 0.757
    std: 0.011
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.37
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_display: Sep 2023
    date_iso: '2023-09-18'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.757
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN (Supervised EdgePred)
    model_key: d&d-node +vn
    model_plain: GIN (Supervised EdgePred)
    value: 0.7556
    std: 0.0068
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.04062'
    title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising
      and Cross-Modal Distillation'
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7556
    sort_std: 0.0068
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AttentiveFP
    model_key: attentivefp
    model_plain: AttentiveFP
    value: 0.637
    std: 0.002
    paper_value: 0.637
    paper_std: 0.002
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.743
    at_pub_std: null
    at_pub_source_arxiv: '2109.11730'
    at_pub_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    at_pub_source_date_iso: '2021-09-24'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-09-24'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.10599999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.743
    true_std: null
    value_gap_source_arxiv: '2109.11730'
    value_gap_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.10599999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.743
    sort_std: null
    global_rank: 12
    paper_rank: 139
    rank_delta: 127
    rank_delta_abs: 127
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular
      Property Prediction'
    comparison_source_arxiv: '2109.11730'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.653
    std: 0.001
    paper_value: 0.653
    paper_std: 0.001
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.735
    at_pub_std: 0.002
    at_pub_source_arxiv: '2011.15069'
    at_pub_source_title: Graph convolutions that can finally model local structure
    at_pub_source_date_iso: '2020-11-30'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-11-30'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.08199999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.735
    true_std: 0.002
    value_gap_source_arxiv: '2011.15069'
    value_gap_source_title: Graph convolutions that can finally model local structure
    value_gap_source_is_current_paper: false
    value_gap: 0.08199999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.735
    sort_std: 0.002
    global_rank: 18
    paper_rank: 108
    rank_delta: 90
    rank_delta_abs: 90
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph convolutions that can finally model local structure
    comparison_source_arxiv: '2011.15069'
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.627
    std: 0.006
    paper_value: 0.627
    paper_std: 0.006
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.711
    at_pub_std: 0.014
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.08399999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.711
    true_std: 0.014
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.08399999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.711
    sort_std: 0.014
    global_rank: 37
    paper_rank: 170
    rank_delta: 133
    rank_delta_abs: 133
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.657
    std: 0.006
    paper_value: 0.657
    paper_std: 0.006
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.634
    at_pub_std: 0.007
    at_pub_source_arxiv: '2112.03806'
    at_pub_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
    at_pub_source_date_iso: '2021-12-07'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.02300000000000002
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7095
    true_std: 0.0027
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.05249999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7095
    sort_std: 0.0027
    global_rank: 38
    paper_rank: 101
    rank_delta: 63
    rank_delta_abs: 63
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural
      Network'
    comparison_source_arxiv: '2112.03806'
    is_best: false
    is_std_outlier: false
  - model: GROVER
    model_key: grover
    model_plain: GROVER
    value: 0.653
    std: 0.005
    paper_value: 0.653
    paper_std: 0.005
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.708
    at_pub_std: 0.015
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.05499999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.708
    true_std: 0.015
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.05499999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.708
    sort_std: 0.015
    global_rank: 40
    paper_rank: 108
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.628
    std: 0.002
    paper_value: 0.628
    paper_std: 0.002
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.696
    at_pub_std: 0.023
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.06799999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.696
    true_std: 0.023
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.06799999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.696
    sort_std: 0.023
    global_rank: 49
    paper_rank: 170
    rank_delta: 121
    rank_delta_abs: 121
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: GEM
    model_key: gem
    model_plain: GEM
    value: 0.692
    std: 0.004
    paper_value: 0.692
    paper_std: 0.004
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.692
    true_std: 0.004
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.692
    sort_std: 0.004
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
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.627
    std: 0.001
    paper_value: 0.627
    paper_std: 0.001
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.689
    at_pub_std: 0.01
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.061999999999999944
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.689
    true_std: 0.01
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.061999999999999944
    has_value_note: false
    value_note: ''
    sort_value: 0.689
    sort_std: 0.01
    global_rank: 58
    paper_rank: 170
    rank_delta: 112
    rank_delta_abs: 112
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.649
    std: 0.002
    paper_value: 0.649
    paper_std: 0.002
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
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.608
    at_pub_std: 0.005
    at_pub_source_arxiv: '2209.15101'
    at_pub_source_title: Improving Molecular Pretraining with Complementary Featurizations
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.041000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6775
    true_std: 0.0041
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.02849999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6775
    sort_std: 0.0041
    global_rank: 70
    paper_rank: 116
    rank_delta: 46
    rank_delta_abs: 46
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Improving Molecular Pretraining with Complementary Featurizations
    comparison_source_arxiv: '2209.15101'
    is_best: false
    is_std_outlier: false
  - model: D-MPNN
    model_key: d-mpnn
    model_plain: D-MPNN
    value: 0.655
    std: 0.003
    paper_value: 0.655
    paper_std: 0.003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.655
    true_std: 0.003
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.655
    sort_std: 0.003
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
  - model: MOLTOP
    model_key: moltop
    model_plain: MOLTOP
    value: 0.644
    std: 0.003
    paper_value: 0.644
    paper_std: 0.003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: mixed
    feature_source_evidence: utilizing both topological descriptors and simple atom
      and bonds features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.644
    true_std: 0.003
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.644
    sort_std: 0.003
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
  - model: Adding atoms and bonds features
    model_key: adding atoms and bonds features
    model_plain: Adding atoms and bonds features
    value: 0.635
    std: 0.003
    paper_value: 0.635
    paper_std: 0.003
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
    input_feature_source: mixed
    feature_source_evidence: Adding atoms and bonds features
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.635
    true_std: 0.003
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.635
    sort_std: 0.003
    global_rank: 143
    paper_rank: 143
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
    value: 0.631
    std: 0.004
    paper_value: 0.631
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: Pretr. Yes
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.631
    at_pub_std: 0.004
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.631
    true_std: 0.004
    value_gap_source_arxiv: '2110.07728'
    value_gap_source_title: 16 Pre-training Molecular Graph Representation with 3D
      Geometry
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.631
    sort_std: 0.004
    global_rank: 163
    paper_rank: 163
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ECFP
    model_key: ecfp
    model_plain: ECFP
    value: 0.604
    std: 0.004
    paper_value: 0.604
    paper_std: 0.004
    metric: ROC-AUC
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
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.604
    true_std: 0.004
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.604
    sort_std: 0.004
    global_rank: 198
    paper_rank: 198
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Adding topological edge features
    model_key: adding topological edge features
    model_plain: Adding topological edge features
    value: 0.603
    std: 0.005
    paper_value: 0.603
    paper_std: 0.005
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
    input_feature_source: mixed
    feature_source_evidence: Adding topological edge features
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.603
    true_std: 0.005
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.603
    sort_std: 0.005
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
  - model: LTP
    model_key: ltp
    model_plain: LTP
    value: 0.6
    std: 0.004
    paper_value: 0.6
    paper_std: 0.004
    metric: ROC-AUC
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
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.6
    true_std: 0.004
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6
    sort_std: 0.004
    global_rank: 200
    paper_rank: 200
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LDP
    model_key: ldp
    model_plain: LDP
    value: 0.595
    std: 0.004
    paper_value: 0.595
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.595
    true_std: 0.004
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.595
    sort_std: 0.004
    global_rank: 201
    paper_rank: 201
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LDP, 50 bins
    model_key: ldp, 50 bins
    model_plain: LDP, 50 bins
    value: 0.595
    std: 0.004
    paper_value: 0.595
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.595
    true_std: 0.004
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.595
    sort_std: 0.004
    global_rank: 202
    paper_rank: 202
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: molecular fingerprint
    model_key: molecular fingerprint
    model_plain: molecular fingerprint
    value: 0.575
    std: 0.001
    paper_value: 0.575
    paper_std: 0.001
    metric: ROC-AUC
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
    protocol_note: Scaffold split provided by OGB
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
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
    true_value: 0.575
    true_std: 0.001
    value_gap_source_arxiv: '2407.12136'
    value_gap_source_title: Molecular Topological Profile (MOLTOP) - Simple and Strong
      Baseline for Molecular Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.575
    sort_std: 0.001
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
  - *id003
- benchmark: LRGB
  datasets:
  - *id004
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
    - dataset: ToxCast
      dataset_slug: toxcast
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: Peptides-func
      dataset_slug: peptides-func
single_proposed_model: MOLTOP
main_figure: /figures/2407.12136/main_figure.jpegoptim.jpg
---

