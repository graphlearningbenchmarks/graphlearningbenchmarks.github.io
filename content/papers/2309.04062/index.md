---
title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising and
  Cross-Modal Distillation'
arxiv_id: '2309.04062'
source_url: ''
authors:
- name: Sungjun Cho
  orcid: null
  s2_author_id: '2149157242'
  s2_url: null
- name: Dae-Woong Jeong
  orcid: null
  s2_author_id: '2238633053'
  s2_url: null
- name: Sung Moon Ko
  orcid: null
  s2_author_id: '2238640140'
  s2_url: null
- name: Jinwoo Kim
  orcid: null
  s2_author_id: '2144171168'
  s2_url: null
- name: Sehui Han
  orcid: null
  s2_author_id: '2175361381'
  s2_url: null
- name: Seunghoon Hong
  orcid: null
  s2_author_id: '2241528'
  s2_url: null
- name: Honglak Lee
  orcid: null
  s2_author_id: '1697141'
  s2_url: null
- name: Moontae Lee
  orcid: null
  s2_author_id: '3056520'
  s2_url: null
published_date: Sep 8, 2023
published_date_iso: '2023-09-08'
published_venue: AAAI 2023
published_conference: AAAI 2023
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Pretraining molecular representations from large unlabeled data is essential
  for molecular property prediction due to the high cost of obtaining ground-truth
  labels. While there exist various 2D graph-based molecular pretraining approaches,
  these methods struggle to show statistically significant gains in predictive performance.
  Recent work have thus instead proposed 3D conformer-based pretraining under the
  task of denoising, which led to promising results. During downstream finetuning,
  however, models trained with 3D conformers require accurate atom-coordinates of
  previously unseen molecules, which are computationally expensive to acquire at scale.
  In light of this limitation, we propose D&D, a self-supervised molecular representation
  learning framework that pretrains a 2D graph encoder by distilling representations
  from a 3D denoiser. With denoising followed by cross-modal knowledge distillation,
  our approach enjoys use of knowledge obtained from denoising as well as painless
  application to downstream tasks with no access to accurate conformers. Experiments
  on real-world molecular property prediction datasets show that the graph encoder
  trained via D&D can infer 3D information based on the 2D graph and shows superior
  performance and label-efficiency against other baselines.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 8
  total: 9
task_categories:
- graph_classification
- graph_regression
experiment_scopes:
- graph-level
results:
- &id002
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
  - model: D&D-Graph +vn
    model_key: d&d-graph +vn
    model_plain: D&D-Graph +vn
    value: 0.7271
    std: 0.0721
    paper_value: 0.7271
    paper_std: 0.0721
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BACE task using scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7271
    true_std: 0.0721
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7271
    sort_std: 0.0721
    global_rank: 254
    paper_rank: 254
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +vn
    model_key: randinit +vn
    model_plain: RandInit +vn
    value: 0.7078
    std: 0.0284
    paper_value: 0.7078
    paper_std: 0.0284
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
    protocol_note: OGB BACE task using scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7078
    true_std: 0.0284
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7078
    sort_std: 0.0284
    global_rank: 269
    paper_rank: 269
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +mp
    model_key: d&d-graph +mp
    model_plain: D&D-Graph +mp
    value: 0.6906
    std: 0.1339
    paper_value: 0.6906
    paper_std: 0.1339
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BACE task using scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6906
    true_std: 0.1339
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6906
    sort_std: 0.1339
    global_rank: 277
    paper_rank: 277
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: d&d-node +vn
    model_plain: D&D-Node +vn
    value: 0.6649
    std: 0.146
    paper_value: 0.6649
    paper_std: 0.146
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BACE task using scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6649
    true_std: 0.146
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6649
    sort_std: 0.146
    global_rank: 285
    paper_rank: 285
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +mp
    model_key: randinit +mp
    model_plain: RandInit +mp
    value: 0.636
    std: 0.1055
    paper_value: 0.636
    paper_std: 0.1055
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
    protocol_note: OGB BACE task using scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.636
    true_std: 0.1055
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.636
    sort_std: 0.1055
    global_rank: 290
    paper_rank: 290
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +vn
    model_key: 3dinfomax +vn
    model_plain: 3DInfomax +vn
    value: 0.6016
    std: 0.405
    paper_value: 0.6016
    paper_std: 0.405
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
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BACE task using scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6016
    true_std: 0.405
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6016
    sort_std: 0.405
    global_rank: 299
    paper_rank: 299
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: D&D-Node +mp
    model_key: d&d-node +mp
    model_plain: D&D-Node +mp
    value: 0.5882
    std: 0.2827
    paper_value: 0.5882
    paper_std: 0.2827
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BACE task using scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5882
    true_std: 0.2827
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5882
    sort_std: 0.2827
    global_rank: 301
    paper_rank: 301
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +mp
    model_key: 3dinfomax +mp
    model_plain: 3DInfomax +mp
    value: 0.5701
    std: 0.0924
    paper_value: 0.5701
    paper_std: 0.0924
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
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BACE task using scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5701
    true_std: 0.0924
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5701
    sort_std: 0.0924
    global_rank: 302
    paper_rank: 302
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
- &id003
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
  - model: D&D-Node +vn
    model_key: d&d-node +vn
    model_plain: D&D-Node +vn
    value: 0.6788
    std: 0.0068
    paper_value: 0.6788
    paper_std: 0.0068
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BBBP scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6788
    true_std: 0.0068
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6788
    sort_std: 0.0068
    global_rank: 195
    paper_rank: 195
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +mp
    model_key: d&d-graph +mp
    model_plain: D&D-Graph +mp
    value: 0.6775
    std: 0.0117
    paper_value: 0.6775
    paper_std: 0.0117
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BBBP scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6775
    true_std: 0.0117
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6775
    sort_std: 0.0117
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
  - model: D&D-Node +mp
    model_key: d&d-node +mp
    model_plain: D&D-Node +mp
    value: 0.6754
    std: 0.0028
    paper_value: 0.6754
    paper_std: 0.0028
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BBBP scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6754
    true_std: 0.0028
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6754
    sort_std: 0.0028
    global_rank: 209
    paper_rank: 209
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +vn
    model_key: d&d-graph +vn
    model_plain: D&D-Graph +vn
    value: 0.6714
    std: 0.0144
    paper_value: 0.6714
    paper_std: 0.0144
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BBBP scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6714
    true_std: 0.0144
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6714
    sort_std: 0.0144
    global_rank: 219
    paper_rank: 219
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +mp
    model_key: randinit +mp
    model_plain: RandInit +mp
    value: 0.6453
    std: 0.0153
    paper_value: 0.6453
    paper_std: 0.0153
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
    protocol_note: OGB BBBP scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6453
    true_std: 0.0153
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6453
    sort_std: 0.0153
    global_rank: 268
    paper_rank: 268
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +vn
    model_key: 3dinfomax +vn
    model_plain: 3DInfomax +vn
    value: 0.6358
    std: 0.0088
    paper_value: 0.6358
    paper_std: 0.0088
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
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BBBP scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6358
    true_std: 0.0088
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6358
    sort_std: 0.0088
    global_rank: 278
    paper_rank: 278
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +vn
    model_key: randinit +vn
    model_plain: RandInit +vn
    value: 0.6305
    std: 0.0066
    paper_value: 0.6305
    paper_std: 0.0066
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
    protocol_note: OGB BBBP scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6305
    true_std: 0.0066
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6305
    sort_std: 0.0066
    global_rank: 282
    paper_rank: 282
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +mp
    model_key: 3dinfomax +mp
    model_plain: 3DInfomax +mp
    value: 0.6238
    std: 0.012
    paper_value: 0.6238
    paper_std: 0.012
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
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB BBBP scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6238
    true_std: 0.012
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6238
    sort_std: 0.012
    global_rank: 286
    paper_rank: 286
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
  dataset: ClinTox
  rows:
  - model: EdgePrompt+
    model_key: se(3)-i mpph
    model_plain: EdgePrompt+
    value: 0.993
    std: 0.004
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
    global_rank: 1
    sort_value: 0.993
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: ka-gcn
    model_plain: EdgePrompt+
    value: 0.992
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
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.992
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EdgePrompt+
    model_key: ka-gat
    model_plain: EdgePrompt+
    value: 0.991
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
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.991
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: 3DInfomax +mp
    model_key: 3dinfomax +mp
    model_plain: 3DInfomax +mp
    value: 0.6919
    std: 0.0419
    paper_value: 0.6919
    paper_std: 0.0419
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6919
    true_std: 0.0419
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6919
    sort_std: 0.0419
    global_rank: 178
    paper_rank: 178
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +vn
    model_key: randinit +vn
    model_plain: RandInit +vn
    value: 0.6834
    std: 0.0468
    paper_value: 0.6834
    paper_std: 0.0468
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
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6834
    true_std: 0.0468
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6834
    sort_std: 0.0468
    global_rank: 182
    paper_rank: 182
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +vn
    model_key: 3dinfomax +vn
    model_plain: 3DInfomax +vn
    value: 0.6815
    std: 0.0361
    paper_value: 0.6815
    paper_std: 0.0361
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6815
    true_std: 0.0361
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6815
    sort_std: 0.0361
    global_rank: 183
    paper_rank: 183
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +mp
    model_key: d&d-graph +mp
    model_plain: D&D-Graph +mp
    value: 0.6761
    std: 0.0211
    paper_value: 0.6761
    paper_std: 0.0211
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6761
    true_std: 0.0211
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6761
    sort_std: 0.0211
    global_rank: 188
    paper_rank: 188
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +vn
    model_key: d&d-graph +vn
    model_plain: D&D-Graph +vn
    value: 0.671
    std: 0.0429
    paper_value: 0.671
    paper_std: 0.0429
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.671
    true_std: 0.0429
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.671
    sort_std: 0.0429
    global_rank: 193
    paper_rank: 193
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: d&d-node +vn
    model_plain: D&D-Node +vn
    value: 0.6594
    std: 0.0502
    paper_value: 0.6594
    paper_std: 0.0502
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6594
    true_std: 0.0502
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6594
    sort_std: 0.0502
    global_rank: 195
    paper_rank: 195
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +mp
    model_key: randinit +mp
    model_plain: RandInit +mp
    value: 0.6141
    std: 0.029
    paper_value: 0.6141
    paper_std: 0.029
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
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6141
    true_std: 0.029
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6141
    sort_std: 0.029
    global_rank: 216
    paper_rank: 216
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +mp
    model_key: d&d-node +mp
    model_plain: D&D-Node +mp
    value: 0.5825
    std: 0.0257
    paper_value: 0.5825
    paper_std: 0.0257
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5825
    true_std: 0.0257
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5825
    sort_std: 0.0257
    global_rank: 227
    paper_rank: 227
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
- &id007
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
  - model: D&D-Graph +mp
    model_key: d&d-graph +mp
    model_plain: D&D-Graph +mp
    value: 0.9276
    std: 0.0562
    paper_value: 0.9276
    paper_std: 0.0562
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: OGB ESOL task using standard scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9276
    true_std: 0.0562
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9276
    sort_std: 0.0562
    global_rank: 65
    paper_rank: 65
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +vn
    model_key: d&d-graph +vn
    model_plain: D&D-Graph +vn
    value: 0.9934
    std: 0.0203
    paper_value: 0.9934
    paper_std: 0.0203
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: OGB ESOL task using standard scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9934
    true_std: 0.0203
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9934
    sort_std: 0.0203
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
  - model: D&D-Node +mp
    model_key: d&d-node +mp
    model_plain: D&D-Node +mp
    value: 1.0097
    std: 0.0381
    paper_value: 1.0097
    paper_std: 0.0381
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: OGB ESOL task using standard scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0097
    true_std: 0.0381
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0097
    sort_std: 0.0381
    global_rank: 76
    paper_rank: 76
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +mp
    model_key: randinit +mp
    model_plain: RandInit +mp
    value: 1.0491
    std: 0.0363
    paper_value: 1.0491
    paper_std: 0.0363
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: OGB ESOL task using standard scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0491
    true_std: 0.0363
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0491
    sort_std: 0.0363
    global_rank: 80
    paper_rank: 80
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: d&d-node +vn
    model_plain: D&D-Node +vn
    value: 1.0862
    std: 0.0887
    paper_value: 1.0862
    paper_std: 0.0887
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: OGB ESOL task using standard scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0862
    true_std: 0.0887
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0862
    sort_std: 0.0887
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
  - model: RandInit +vn
    model_key: randinit +vn
    model_plain: RandInit +vn
    value: 1.1074
    std: 0.0735
    paper_value: 1.1074
    paper_std: 0.0735
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: OGB ESOL task using standard scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.1074
    true_std: 0.0735
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.1074
    sort_std: 0.0735
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
  - model: 3DInfomax +vn
    model_key: 3dinfomax +vn
    model_plain: 3DInfomax +vn
    value: 1.5246
    std: 0.1092
    paper_value: 1.5246
    paper_std: 0.1092
    metric: RMSE
    higher_is_better: false
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
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: OGB ESOL task using standard scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.5246
    true_std: 0.1092
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.5246
    sort_std: 0.1092
    global_rank: 120
    paper_rank: 120
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +mp
    model_key: 3dinfomax +mp
    model_plain: 3DInfomax +mp
    value: 2.0037
    std: 0.1076
    paper_value: 2.0037
    paper_std: 0.1076
    metric: RMSE
    higher_is_better: false
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
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: OGB ESOL task using standard scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.0037
    true_std: 0.1076
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.0037
    sort_std: 0.1076
    global_rank: 129
    paper_rank: 129
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
- &id008
  dataset: FreeSolv
  rows:
  - model: D&D-Node +vn
    model_key: se(3)-i mpph
    model_plain: D&D-Node +vn
    value: 0.354
    std: 0.053
    metric: RMSE
    higher_is_better: false
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
    global_rank: 1
    sort_value: 0.354
    sort_std: 0.053
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: ecfp-4 + rf
    model_plain: D&D-Node +vn
    value: 0.56
    std: 0.066
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
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
    feature_source_evidence: trained on ECFP-4 fingerprints
    is_global_top: true
    global_rank: 2
    sort_value: 0.56
    sort_std: 0.066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: geomgcl
    model_plain: D&D-Node +vn
    value: 0.866
    std: null
    metric: RMSE
    higher_is_better: false
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
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: The model uses a 2D-3D geometric contrastive scheme to
      bridge knowledge between 2D chemical semantics and 3D spatial information.
    is_global_top: true
    global_rank: 3
    sort_value: 0.866
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +mp
    model_key: d&d-graph +mp
    model_plain: D&D-Graph +mp
    value: 2.6814
    std: 0.0867
    paper_value: 2.6814
    paper_std: 0.0867
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.6814
    true_std: 0.0867
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.6814
    sort_std: 0.0867
    global_rank: 67
    paper_rank: 67
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +vn
    model_key: d&d-graph +vn
    model_plain: D&D-Graph +vn
    value: 2.7004
    std: 0.0572
    paper_value: 2.7004
    paper_std: 0.0572
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.7004
    true_std: 0.0572
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.7004
    sort_std: 0.0572
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
  - model: D&D-Node +mp
    model_key: d&d-node +mp
    model_plain: D&D-Node +mp
    value: 3.2935
    std: 0.2872
    paper_value: 3.2935
    paper_std: 0.2872
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.2935
    true_std: 0.2872
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.2935
    sort_std: 0.2872
    global_rank: 95
    paper_rank: 95
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: d&d-node +vn
    model_plain: D&D-Node +vn
    value: 3.4056
    std: 0.2221
    paper_value: 3.4056
    paper_std: 0.2221
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.4056
    true_std: 0.2221
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.4056
    sort_std: 0.2221
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
  - model: RandInit +vn
    model_key: randinit +vn
    model_plain: RandInit +vn
    value: 3.5325
    std: 0.0453
    paper_value: 3.5325
    paper_std: 0.0453
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.5325
    true_std: 0.0453
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.5325
    sort_std: 0.0453
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
  - model: RandInit +mp
    model_key: randinit +mp
    model_plain: RandInit +mp
    value: 3.6445
    std: 0.0734
    paper_value: 3.6445
    paper_std: 0.0734
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.6445
    true_std: 0.0734
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.6445
    sort_std: 0.0734
    global_rank: 101
    paper_rank: 101
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +vn
    model_key: 3dinfomax +vn
    model_plain: 3DInfomax +vn
    value: 4.258
    std: 0.3782
    paper_value: 4.258
    paper_std: 0.3782
    metric: RMSE
    higher_is_better: false
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
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 4.258
    true_std: 0.3782
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 4.258
    sort_std: 0.3782
    global_rank: 108
    paper_rank: 108
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +mp
    model_key: 3dinfomax +mp
    model_plain: 3DInfomax +mp
    value: 4.6854
    std: 0.4345
    paper_value: 4.6854
    paper_std: 0.4345
    metric: RMSE
    higher_is_better: false
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
    source_ref: 3DInfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 4.6854
    true_std: 0.4345
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 4.6854
    sort_std: 0.4345
    global_rank: 112
    paper_rank: 112
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
- &id005
  dataset: SIDER
  rows:
  - model: DGI
    model_key: ka-gat
    model_plain: DGI
    value: 0.847
    std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.847
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DGI
    model_key: ka-gcn
    model_plain: DGI
    value: 0.842
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.842
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: graphkan
    model_plain: DGI
    value: 0.837
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_display: Apr 2026
    date_iso: '2026-04-17'
    venue: Journal of Chemical Theory and Computation
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.837
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +vn
    model_key: d&d-node +vn
    model_plain: D&D-Node +vn
    value: 0.6257
    std: 0.0106
    paper_value: 0.6257
    paper_std: 0.0106
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6257
    true_std: 0.0106
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6257
    sort_std: 0.0106
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
  - model: D&D-Graph +vn
    model_key: d&d-graph +vn
    model_plain: D&D-Graph +vn
    value: 0.6117
    std: 0.0229
    paper_value: 0.6117
    paper_std: 0.0229
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6117
    true_std: 0.0229
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6117
    sort_std: 0.0229
    global_rank: 139
    paper_rank: 139
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Node +mp
    model_key: d&d-node +mp
    model_plain: D&D-Node +mp
    value: 0.6017
    std: 0.0113
    paper_value: 0.6017
    paper_std: 0.0113
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6017
    true_std: 0.0113
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6017
    sort_std: 0.0113
    global_rank: 178
    paper_rank: 178
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +mp
    model_key: randinit +mp
    model_plain: RandInit +mp
    value: 0.6005
    std: 0.0058
    paper_value: 0.6005
    paper_std: 0.0058
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
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6005
    true_std: 0.0058
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6005
    sort_std: 0.0058
    global_rank: 181
    paper_rank: 181
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +vn
    model_key: 3dinfomax +vn
    model_plain: 3DInfomax +vn
    value: 0.6004
    std: 0.0216
    paper_value: 0.6004
    paper_std: 0.0216
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
    source_ref: stark20223dinfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6004
    true_std: 0.0216
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6004
    sort_std: 0.0216
    global_rank: 182
    paper_rank: 182
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +mp
    model_key: d&d-graph +mp
    model_plain: D&D-Graph +mp
    value: 0.5988
    std: 0.0049
    paper_value: 0.5988
    paper_std: 0.0049
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5988
    true_std: 0.0049
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5988
    sort_std: 0.0049
    global_rank: 187
    paper_rank: 187
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +mp
    model_key: 3dinfomax +mp
    model_plain: 3DInfomax +mp
    value: 0.5979
    std: 0.0086
    paper_value: 0.5979
    paper_std: 0.0086
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
    source_ref: stark20223dinfomax
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5979
    true_std: 0.0086
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5979
    sort_std: 0.0086
    global_rank: 190
    paper_rank: 190
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +vn
    model_key: randinit +vn
    model_plain: RandInit +vn
    value: 0.593
    std: 0.0036
    paper_value: 0.593
    paper_std: 0.0036
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
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.593
    true_std: 0.0036
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.593
    sort_std: 0.0036
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
  - model: D&D-Node +vn
    model_key: d&d-node +vn
    model_plain: D&D-Node +vn
    value: 0.7556
    std: 0.0068
    paper_value: 0.7556
    paper_std: 0.0068
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB Tox21 task using standard split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7556
    true_std: 0.0068
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7556
    sort_std: 0.0068
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
  - model: D&D-Graph +vn
    model_key: d&d-graph +vn
    model_plain: D&D-Graph +vn
    value: 0.7554
    std: 0.0003
    paper_value: 0.7554
    paper_std: 0.0003
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB Tox21 task using standard split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7554
    true_std: 0.0003
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7554
    sort_std: 0.0003
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
  - model: D&D-Node +mp
    model_key: d&d-node +mp
    model_plain: D&D-Node +mp
    value: 0.7549
    std: 0.0055
    paper_value: 0.7549
    paper_std: 0.0055
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB Tox21 task using standard split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7549
    true_std: 0.0055
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7549
    sort_std: 0.0055
    global_rank: 203
    paper_rank: 203
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: D&D-Graph +mp
    model_key: d&d-graph +mp
    model_plain: D&D-Graph +mp
    value: 0.7541
    std: 0.0014
    paper_value: 0.7541
    paper_std: 0.0014
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB Tox21 task using standard split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7541
    true_std: 0.0014
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7541
    sort_std: 0.0014
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
  - model: RandInit +mp
    model_key: randinit +mp
    model_plain: RandInit +mp
    value: 0.7219
    std: 0.0035
    paper_value: 0.7219
    paper_std: 0.0035
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
    protocol_note: OGB Tox21 task using standard split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7219
    true_std: 0.0035
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7219
    sort_std: 0.0035
    global_rank: 283
    paper_rank: 283
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +vn
    model_key: randinit +vn
    model_plain: RandInit +vn
    value: 0.719
    std: 0.0051
    paper_value: 0.719
    paper_std: 0.0051
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
    protocol_note: OGB Tox21 task using standard split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.719
    true_std: 0.0051
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.719
    sort_std: 0.0051
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
  - model: 3DInfomax +vn
    model_key: 3dinfomax +vn
    model_plain: 3DInfomax +vn
    value: 0.6979
    std: 0.0066
    paper_value: 0.6979
    paper_std: 0.0066
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB Tox21 task using standard split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6979
    true_std: 0.0066
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6979
    sort_std: 0.0066
    global_rank: 299
    paper_rank: 299
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +mp
    model_key: 3dinfomax +mp
    model_plain: 3DInfomax +mp
    value: 0.6925
    std: 0.0114
    paper_value: 0.6925
    paper_std: 0.0114
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB Tox21 task using standard split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6925
    true_std: 0.0114
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6925
    sort_std: 0.0114
    global_rank: 302
    paper_rank: 302
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
- &id006
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
  - model: D&D-Node +vn
    model_key: d&d-node +vn
    model_plain: D&D-Node +vn
    value: 0.7556
    std: 0.0068
    paper_value: 0.7556
    paper_std: 0.0068
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7556
    true_std: 0.0068
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7556
    sort_std: 0.0068
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
  - model: D&D-Graph +vn
    model_key: d&d-graph +vn
    model_plain: D&D-Graph +vn
    value: 0.7554
    std: 0.0003
    paper_value: 0.7554
    paper_std: 0.0003
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7554
    true_std: 0.0003
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7554
    sort_std: 0.0003
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
  - model: D&D-Node +mp
    model_key: d&d-node +mp
    model_plain: D&D-Node +mp
    value: 0.7549
    std: 0.0055
    paper_value: 0.7549
    paper_std: 0.0055
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7549
    true_std: 0.0055
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7549
    sort_std: 0.0055
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
  - model: D&D-Graph +mp
    model_key: d&d-graph +mp
    model_plain: D&D-Graph +mp
    value: 0.7541
    std: 0.0014
    paper_value: 0.7541
    paper_std: 0.0014
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7541
    true_std: 0.0014
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7541
    sort_std: 0.0014
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandInit +mp
    model_key: randinit +mp
    model_plain: RandInit +mp
    value: 0.7219
    std: 0.0035
    paper_value: 0.7219
    paper_std: 0.0035
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
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7219
    true_std: 0.0035
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7219
    sort_std: 0.0035
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
  - model: RandInit +vn
    model_key: randinit +vn
    model_plain: RandInit +vn
    value: 0.719
    std: 0.0051
    paper_value: 0.719
    paper_std: 0.0051
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
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.719
    true_std: 0.0051
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.719
    sort_std: 0.0051
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
  - model: 3DInfomax +vn
    model_key: 3dinfomax +vn
    model_plain: 3DInfomax +vn
    value: 0.6979
    std: 0.0066
    paper_value: 0.6979
    paper_std: 0.0066
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6979
    true_std: 0.0066
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6979
    sort_std: 0.0066
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3DInfomax +mp
    model_key: 3dinfomax +mp
    model_plain: 3DInfomax +mp
    value: 0.6925
    std: 0.0114
    paper_value: 0.6925
    paper_std: 0.0114
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Scaffold split
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    published_venue: AAAI 2023
    published_conference: AAAI 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6925
    true_std: 0.0114
    value_gap_source_arxiv: '2309.04062'
    value_gap_source_title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining
      via Denoising and Cross-Modal Distillation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6925
    sort_std: 0.0114
    global_rank: 51
    paper_rank: 51
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
  - *id004
  - *id005
  - *id006
  - *id007
  - *id008
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: Tox21
      dataset_slug: tox21
    - dataset: BACE
      dataset_slug: bace
    - dataset: BBBP
      dataset_slug: bbbp
    - dataset: ClinTox
      dataset_slug: clintox
    - dataset: SIDER
      dataset_slug: sider
    - dataset: ToxCast
      dataset_slug: toxcast
    - dataset: ESOL
      dataset_slug: esol
    - dataset: FreeSolv
      dataset_slug: freesolv
main_figure: /figures/2309.04062/main_figure.jpegoptim.jpg
---

