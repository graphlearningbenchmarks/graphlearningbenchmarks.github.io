---
title: Molecular Contrastive Learning with Chemical Element Knowledge Graph
arxiv_id: '2112.00544'
source_url: ''
authors:
- name: Yin Fang
  orcid: null
  s2_author_id: '2112787103'
  s2_url: null
- name: Qiang Zhang
  orcid: null
  s2_author_id: '2145895211'
  s2_url: null
- name: Haihong Yang
  orcid: null
  s2_author_id: '2118697870'
  s2_url: null
- name: Xiang Zhuang
  orcid: null
  s2_author_id: '2072655893'
  s2_url: null
- name: Shumin Deng
  orcid: null
  s2_author_id: '152931849'
  s2_url: null
- name: Wen Zhang
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Minghai Qin
  orcid: null
  s2_author_id: '39449475'
  s2_url: null
- name: Zhuo Chen
  orcid: null
  s2_author_id: '2283992213'
  s2_url: null
- name: Xiaohui Fan
  orcid: null
  s2_author_id: '2152774386'
  s2_url: null
- name: Huajun Chen
  orcid: null
  s2_author_id: '49178307'
  s2_url: null
published_date: Dec 1, 2021
published_date_iso: '2021-12-01'
published_venue: AAAI 2021
published_conference: AAAI 2021
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Molecular representation learning contributes to multiple downstream tasks
  such as molecular property prediction and drug design. To properly represent molecules,
  graph contrastive learning is a promising paradigm as it utilizes self-supervision
  signals and has no requirements for human annotations. However, prior works fail
  to incorporate fundamental domain knowledge into graph semantics and thus ignore
  the correlations between atoms that have common attributes but are not directly
  connected by bonds. To address these issues, we construct a Chemical Element Knowledge
  Graph (KG) to summarize microscopic associations between elements and propose a
  novel Knowledge-enhanced Contrastive Learning (KCL) framework for molecular representation
  learning. KCL framework consists of three modules. The first module, knowledge-guided
  graph augmentation, augments the original molecular graph based on the Chemical
  Element KG. The second module, knowledge-aware graph representation, extracts molecular
  representations with a common graph encoder for the original molecular graph and
  a Knowledge-aware Message Passing Neural Network (KMPNN) to encode complex information
  in the augmented molecular graph. The final module is a contrastive objective, where
  we maximize agreement between these two views of molecular graphs. Extensive experiments
  demonstrated that KCL obtained superior performances against state-of-the-art baselines
  on eight molecular datasets. Visualization experiments properly interpret what KCL
  has learned from atoms and attributes in the augmented molecular graphs. Our codes
  and data are available at https://github.com/ZJU-Fangyin/KCL.
codebase_url: https://github.com/ZJU-Fangyin/KCL
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- KCL
mrr: 0.0625
adjusted_mrr: 0.0208
mrr_dataset_count: 1
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 1
  total: 9
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ESOL
  rows:
  - model: AMCT
    model_key: mat
    model_plain: AMCT
    value: 0.278
    std: 0.02
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2002.08264'
    title: Molecule Attention Transformer
    date: Feb 19, 2020
    date_display: Feb 2020
    date_iso: '2020-02-19'
    venue: Graph Representation Learning workshop and Machine Learning and the Physical
      Sciences workshop at NeurIPS 2019
    codebase_url: https://github.com/gmum/MAT
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.278
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AMCT
    model_key: smiles
    model_plain: AMCT
    value: 0.356
    std: 0.017
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2002.08264'
    title: Molecule Attention Transformer
    date: Feb 19, 2020
    date_display: Feb 2020
    date_iso: '2020-02-19'
    venue: Graph Representation Learning workshop and Machine Learning and the Physical
      Sciences workshop at NeurIPS 2019
    codebase_url: https://github.com/gmum/MAT
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.356
    sort_std: 0.017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AMCT
    model_key: graphormer-spis
    model_plain: AMCT
    value: 0.484
    std: 0.005
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_display: May 2023
    date_iso: '2023-05-23'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.484
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KCL
    model_key: kcl
    model_plain: KCL
    value: 0.582
    std: null
    paper_value: 0.582
    paper_std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: The model uses a Chemical Element Knowledge Graph (KG)
      to guide augmentation and RotateE for feature initialization.
    table_ref: Table appendix:linear
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Fine-tune protocol evaluation on Scaffold split.
    date: Dec 1, 2021
    date_display: Dec 2021
    date_iso: '2021-12-01'
    published_venue: AAAI 2021
    published_conference: AAAI 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-12-01'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.582
    true_std: null
    value_gap_source_arxiv: '2112.00544'
    value_gap_source_title: Molecular Contrastive Learning with Chemical Element Knowledge
      Graph
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.582
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
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: MoleculeNet
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: ESOL
      dataset_slug: esol
single_proposed_model: KCL
main_figure: /figures/2112.00544/main_figure.jpegoptim.jpg
---

