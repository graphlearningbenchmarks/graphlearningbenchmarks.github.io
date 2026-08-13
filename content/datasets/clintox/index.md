---
title: ClinTox
slug: clintox
benchmark: MoleculeNet
task_type: graph_classification
short_description: Clinical toxicity prediction — FDA-approved vs. failed drugs (2
  tasks).
description: '**2-task graph classification** Clinical toxicity prediction — FDA-approved
  vs. failed drugs (2 tasks). SMILES and labels are fixed; molecular graph featurization
  is implementation-defined. Missing labels are not negatives; report split and featurizer.
  Evaluated by ROC-AUC.'
detailed_description:
  task: Clinical toxicity prediction — FDA-approved vs. failed drugs (2 tasks). The
    primary catalog metric is ROC-AUC.
  data: Clinical toxicity prediction — FDA-approved vs. failed drugs (2 tasks).
  features: MoleculeNet distributes SMILES and targets, not one mandatory graph featurization.
    A graph implementation normally derives atom and bond fields with RDKit or DeepChem;
    results depend on featurizer, salt handling, stereochemistry, and invalid-molecule
    policy.
  splits_and_evaluation: 'The catalog records these protocols or variants: Scaffold
    split. Evaluation uses ROC-AUC (higher is better). Exact masks or folds must come
    from the cited release.'
  quirks_and_pitfalls: Small samples, imbalance, missing assay labels, duplicate compounds,
    and scaffold leakage are common. Missing labels are not negatives. Always report
    split algorithm, featurizer, metric aggregation, and dataset version; random and
    scaffold results are not comparable.
sources:
- title: MoleculeNet benchmark
  arxiv_id: '1703.00564'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric ClinTox loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
  kind: implementation_documentation
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 2
result_count: 315
best_model:
  model: SE(3)-I MPPH
  value: 0.993
  metric: ROC-AUC
  arxiv_id: '2312.07633'
  paper_title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
    Molecular Property Prediction
papers:
- arxiv_id: '2604.16586'
  title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
    Prediction in the Foundation Model Era
  date_iso: '2026-04-17'
  venue: ''
- arxiv_id: '2602.05567'
  title: 'MAGPrompt: Message-Adaptive Graph Prompt Tuning for Graph Neural Networks'
  date_iso: '2026-02-05'
  venue: ''
- arxiv_id: '2602.01771'
  title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural Understanding'
  date_iso: '2026-02-02'
  venue: ''
- arxiv_id: '2510.07289'
  title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D Graph Encoder'
  date_iso: '2025-10-08'
  venue: ''
- arxiv_id: '2503.04362'
  title: A Generalist Cross-Domain Molecular Learning Framework for Structure-Based
    Drug Discovery
  date_iso: '2025-03-06'
  venue: ''
- arxiv_id: '2501.01073'
  title: Graph Generative Pre-trained Transformer
  date_iso: '2025-01-02'
  venue: ICML 2025
- arxiv_id: '2412.15589'
  title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
    Graph Information Bottleneck
  date_iso: '2024-12-20'
  venue: AAAI 2024
- arxiv_id: '2412.07407'
  title: 'Towards Graph Foundation Models: A Study on the Generalization of Positional
    and Structural Encodings'
  date_iso: '2024-12-10'
  venue: TMLR 2024
- arxiv_id: '2410.10365'
  title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
    Samples'
  date_iso: '2024-10-14'
  venue: ''
- arxiv_id: '2406.00403'
  title: Dual-perspective Cross Contrastive Learning in Graph Transformers
  date_iso: '2024-06-01'
  venue: ''
- arxiv_id: '2405.10343'
  title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view Molecular
    Representation Learning'
  date_iso: '2024-05-15'
  venue: ICML 2024
- arxiv_id: '2405.05665'
  title: 'SubGDiff: A Subgraph Diffusion Model to Improve Molecular Representation
    Learning'
  date_iso: '2024-05-09'
  venue: NeurIPS 2024
- arxiv_id: '2405.01350'
  title: Community-Invariant Graph Contrastive Learning
  date_iso: '2024-05-02'
  venue: ICML 2024
- arxiv_id: '2404.15806'
  title: 'Where to Mask: Structure-Guided Masking for Graph Masked Autoencoders'
  date_iso: '2024-04-24'
  venue: IJCAI 2024
- arxiv_id: '2404.11568'
  title: On the Scalability of GNNs for Molecular Graphs
  date_iso: '2024-04-17'
  venue: NeurIPS 2024
- arxiv_id: '2403.01400'
  title: Decoupling Weighing and Selecting for Integrating Multiple Graph Pre-training
    Tasks
  date_iso: '2024-03-03'
  venue: ICLR 2024
- arxiv_id: '2402.10380'
  title: Subgraph-level Universal Prompt Tuning
  date_iso: '2024-02-16'
  venue: ''
- arxiv_id: '2402.08023'
  title: 'UGMAE: A Unified Framework for Graph Masked Autoencoders'
  date_iso: '2024-02-12'
  venue: ''
- arxiv_id: '2402.07249'
  title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent Molecular Property
    Prediction: A Systematic Survey'
  date_iso: '2024-02-11'
  venue: ''
- arxiv_id: '2312.13583'
  title: Fine-tuning Graph Neural Networks by Preserving Graph Generative Patterns
  date_iso: '2023-12-21'
  venue: AAAI 2023
- arxiv_id: '2312.07633'
  title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive Molecular
    Property Prediction
  date_iso: '2023-12-12'
  venue: NeurIPS 2023
- arxiv_id: '2311.01038'
  title: 'Better with Less: A Data-Active Perspective on Pre-Training Graph Neural
    Networks'
  date_iso: '2023-11-02'
  venue: NeurIPS 2023
- arxiv_id: '2310.14753'
  title: Rethinking Tokenizer and Decoder in Masked Graph Modeling for Molecules
  date_iso: '2023-10-23'
  venue: NeurIPS 2023
- arxiv_id: '2310.14216'
  title: 'UniMAP: Universal SMILES-Graph Representation Learning'
  date_iso: '2023-10-22'
  venue: ''
- arxiv_id: '2309.10131'
  title: Deep Prompt Tuning for Graph Transformers
  date_iso: '2023-09-18'
  venue: ''
- arxiv_id: '2309.04589'
  title: Motif-aware Attribute Masking for Molecular Graph Pre-training
  date_iso: '2023-09-08'
  venue: ''
- arxiv_id: '2309.04062'
  title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising and
    Cross-Modal Distillation'
  date_iso: '2023-09-08'
  venue: AAAI 2023
- arxiv_id: '2309.02304'
  title: Graph Self-Contrast Representation Learning
  date_iso: '2023-09-05'
  venue: ''
- arxiv_id: '2306.03506'
  title: Subgraph Networks Based Contrastive Learning
  date_iso: '2023-06-06'
  venue: ''
- arxiv_id: '2305.18407'
  title: A Group Symmetric Stochastic Differential Equation Model for Molecule Multi-modal
    Pretraining
  date_iso: '2023-05-28'
  venue: ICML 2023
- arxiv_id: '2305.15745'
  title: Robust Ante-hoc Graph Explainer using Bilevel Optimization
  date_iso: '2023-05-25'
  venue: ''
- arxiv_id: '2303.16458'
  title: When to Pre-Train Graph Neural Networks? From Data Generation Perspective!
  date_iso: '2023-03-29'
  venue: KDD 2023
- arxiv_id: '2209.15240'
  title: Universal Prompt Tuning for Graph Neural Networks
  date_iso: '2022-09-30'
  venue: NeurIPS 2022
- arxiv_id: '2209.15101'
  title: Improving Molecular Pretraining with Complementary Featurizations
  date_iso: '2022-09-29'
  venue: ''
- arxiv_id: '2208.04529'
  title: Motif-based Graph Representation Learning with Application to Chemical Molecules
  date_iso: '2022-08-09'
  venue: ''
- arxiv_id: '2207.08806'
  title: Unified 2D and 3D Pre-Training of Molecular Representations
  date_iso: '2022-07-14'
  venue: KDD 2022
- arxiv_id: '2207.06010'
  title: Does GNN Pretraining Help Molecular Representation?
  date_iso: '2022-07-13'
  venue: NeurIPS 2022
- arxiv_id: '2206.07869'
  title: Let Invariant Rationale Discovery Inspire Graph Contrastive Learning
  date_iso: '2022-06-16'
  venue: ICML 2022
- arxiv_id: '2206.08005'
  title: Evaluating Self-Supervised Learning for Molecular Graph Embeddings
  date_iso: '2022-06-16'
  venue: NeurIPS 2022
- arxiv_id: '2205.15746'
  title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
    Learning
  date_iso: '2022-05-31'
  venue: ICML 2022
- arxiv_id: '2205.10803'
  title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
  date_iso: '2022-05-22'
  venue: KDD 2022
- arxiv_id: '2202.09346'
  title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation and
    Decomposed Fragment Contrast
  date_iso: '2022-02-18'
  venue: ''
- arxiv_id: '2202.02989'
  title: Graph Self-supervised Learning with Accurate Discrepancy Learning
  date_iso: '2022-02-07'
  venue: NeurIPS 2022
- arxiv_id: '2112.03806'
  title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
  date_iso: '2021-12-07'
  venue: ''
- arxiv_id: '2110.07728'
  title: 16 Pre-training Molecular Graph Representation with 3D Geometry
  date_iso: '2021-10-07'
  venue: ICLR 2021
- arxiv_id: '2110.01191'
  title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
  date_iso: '2021-10-04'
  venue: AAAI 2021
- arxiv_id: '2110.00987'
  title: Motif-based Graph Self-Supervised Learning for Molecular Property Prediction
  date_iso: '2021-10-03'
  venue: NeurIPS 2021
- arxiv_id: '2109.11730'
  title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
  date_iso: '2021-09-24'
  venue: AAAI 2021
- arxiv_id: '2106.06130'
  title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
    Prediction'
  date_iso: '2021-06-11'
  venue: ''
- arxiv_id: '2106.04113'
  title: Self-supervised Graph-level Representation Learning with Local and Global
    Structure
  date_iso: '2021-06-08'
  venue: ICML 2021
- arxiv_id: '2106.04509'
  title: 'MoCL: Data-driven Molecular Fingerprint via Knowledge-aware Contrastive
    Learning from Molecular Graph'
  date_iso: '2021-06-05'
  venue: KDD 2021
- arxiv_id: '1905.12265'
  title: Strategies for Pre-training Graph Neural Networks
  date_iso: '2019-05-29'
  venue: ICLR 2019
- arxiv_id: '1801.03226'
  title: Adaptive Graph Convolutional Neural Networks
  date_iso: '2018-01-10'
  venue: AAAI 2018
variants:
- slug: scaffold-split
  name: Scaffold split
  notes: ''
  is_standard: true
  primary_metric: ROC-AUC
  default_metric: ROC-AUC
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 2
  metrics:
  - ROC-AUC
  - Accuracy
  metric_display_names:
  - ROC-AUC
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: SE(3)-I MPPH
    model_plain: SE(3)-I MPPH
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
    date_iso: '2023-12-12'
    date_display: Dec 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.993
    - null
    metric_stds:
    - 0.004
    - null
  - model: KA-GCN
    model_plain: KA-GCN
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
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.992
    - null
    metric_stds:
    - 0.005
    - null
  - model: KA-GAT
    model_plain: KA-GAT
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
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.991
    - null
    metric_stds:
    - 0.005
    - null
  - model: GraphKAN
    model_plain: GraphKAN
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
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.984
    - null
    metric_stds:
    - 0.003
    - null
  - model: UniMAP
    model_plain: UniMAP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.14216'
    title: 'UniMAP: Universal SMILES-Graph Representation Learning'
    date: Oct 22, 2023
    date_iso: '2023-10-22'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.983
    - null
    metric_stds:
    - 0.017
    - null
  - model: KA-GNNs
    model_plain: KA-GNNs
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
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.972
    - null
    metric_stds:
    - 0.001
    - null
  - model: Mol-GDL
    model_plain: Mol-GDL
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
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.966
    - null
    metric_stds:
    - 0.002
    - null
  - model: iMolCLR
    model_plain: iMolCLR
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09346'
    title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation
      and Decomposed Fragment Contrast
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.954
    - null
    metric_stds:
    - 0.011
    - null
  - model: UnifiedMolPretrain
    model_plain: UnifiedMolPretrain
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2207.08806'
    title: Unified 2D and 3D Pre-Training of Molecular Representations
    date: Jul 14, 2022
    date_iso: '2022-07-14'
    date_display: Jul 2022
    codebase_url: https://github.com/teslacool/UnifiedMolPretrain
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.954
    - null
    metric_stds:
    - 0.011
    - null
  - model: Molformer
    model_plain: Molformer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.937
    - null
    metric_stds:
    - null
    - null
  - model: AttentiveFP
    model_plain: AttentiveFP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.933
    - null
    metric_stds:
    - null
    - null
  - model: MolCLR
    model_plain: MolCLR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09346'
    title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation
      and Decomposed Fragment Contrast
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.932
    - null
    metric_stds:
    - 0.017
    - null
  - model: SMPT
    model_plain: SMPT
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
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.927
    - null
    metric_stds:
    - 0.002
    - null
  - model: MoleculeSTM
    model_plain: MoleculeSTM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.07249'
    title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent Molecular
      Property Prediction: A Systematic Survey'
    date: Feb 11, 2024
    date_iso: '2024-02-11'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.925
    - null
    metric_stds:
    - null
    - null
  - model: UniCorn
    model_plain: UniCorn
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.10343'
    title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view Molecular
      Representation Learning'
    date: May 15, 2024
    date_iso: '2024-05-15'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.921
    - null
    metric_stds:
    - 0.004
    - null
  - model: BIT
    model_plain: BIT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.04362'
    title: A Generalist Cross-Domain Molecular Learning Framework for Structure-Based
      Drug Discovery
    date: Mar 6, 2025
    date_iso: '2025-03-06'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.919
    - null
    metric_stds:
    - 0.0133
    - null
  - model: Uni-Mol
    model_plain: Uni-Mol
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
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.919
    - null
    metric_stds:
    - 0.018
    - null
  - model: GeomGCL
    model_plain: GeomGCL
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
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.919
    - null
    metric_stds:
    - null
    - null
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.03806'
    title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
    date: Dec 7, 2021
    date_iso: '2021-12-07'
    date_display: Dec 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.913
    - null
    metric_stds:
    - 0.017
    - null
  - model: MolLM
    model_plain: MolLM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.07249'
    title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent Molecular
      Property Prediction: A Systematic Survey'
    date: Feb 11, 2024
    date_iso: '2024-02-11'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.911
    - null
    metric_stds:
    - null
    - null
  - model: GraphGPS FT
    model_plain: GraphGPS FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 14.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.91
    - null
    metric_stds:
    - 0.046
    - null
  - model: GraphGPS DeepGPT
    model_plain: GraphGPS DeepGPT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.05
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.907
    - null
    metric_stds:
    - 0.044
    - null
  - model: D-MPNN
    model_plain: D-MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.906
    - null
    metric_stds:
    - 0.006
    - null
  - model: GEM
    model_plain: GEM
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
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.901
    - null
    metric_stds:
    - 0.013
    - null
  - model: GeomMPNN
    model_plain: GeomMPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9
    - null
    metric_stds:
    - null
    - null
  - model: MAT
    model_plain: MAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.898
    - null
    metric_stds:
    - null
    - null
  - model: DMPNN
    model_plain: DMPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.897
    - null
    metric_stds:
    - null
    - null
  - model: No pretrain
    model_plain: No pretrain
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.06010'
    title: Does GNN Pretraining Help Molecular Representation?
    date: Jul 13, 2022
    date_iso: '2022-07-13'
    date_display: Jul 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.897
    - null
    metric_stds:
    - 0.0093
    - null
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 2.8
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.893
    - null
    metric_stds:
    - 0.041
    - null
  - model: KV-PLM
    model_plain: KV-PLM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2402.07249'
    title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent Molecular
      Property Prediction: A Systematic Survey'
    date: Feb 11, 2024
    date_iso: '2024-02-11'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.892
    - null
    metric_stds:
    - null
    - null
  - model: GCN-virtual
    model_plain: GCN-virtual
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.03806'
    title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
    date: Dec 7, 2021
    date_iso: '2021-12-07'
    date_display: Dec 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.886
    - null
    metric_stds:
    - 0.021
    - null
  - model: DMPNN
    model_plain: DMPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.886
    - null
    metric_stds:
    - null
    - null
  - model: GROVER_large
    model_plain: GROVER_large
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.884
    - null
    metric_stds:
    - null
    - null
  - model: Graphormer DeepGPT
    model_plain: Graphormer DeepGPT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.884
    - null
    metric_stds:
    - 0.03
    - null
  - model: GIT-Mol
    model_plain: GIT-Mol
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.07249'
    title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent Molecular
      Property Prediction: A Systematic Survey'
    date: Feb 11, 2024
    date_iso: '2024-02-11'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.883
    - null
    metric_stds:
    - null
    - null
  - model: SubGDiff
    model_plain: SubGDiff
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.05665'
    title: 'SubGDiff: A Subgraph Diffusion Model to Improve Molecular Representation
      Learning'
    date: May 9, 2024
    date_iso: '2024-05-09'
    date_display: May 2024
    codebase_url: https://github.com/youjibiying/SubGDiff
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.882
    - null
    metric_stds:
    - 0.0157
    - null
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.03806'
    title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
    date: Dec 7, 2021
    date_iso: '2021-12-07'
    date_display: Dec 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.881
    - null
    metric_stds:
    - 0.025
    - null
  - model: MPNN
    model_plain: MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.879
    - null
    metric_stds:
    - null
    - null
  - model: Node-MPN
    model_plain: Node-MPN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_iso: '2023-12-12'
    date_display: Dec 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.879
    - null
    metric_stds:
    - 0.054
    - null
  - model: StructMAE-L
    model_plain: StructMAE-L
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.15806'
    title: 'Where to Mask: Structure-Guided Masking for Graph Masked Autoencoders'
    date: Apr 24, 2024
    date_iso: '2024-04-24'
    date_display: Apr 2024
    codebase_url: https://github.com/LiuChuang0059/StructMAE
    published_conference: IJCAI 2024
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.879
    - null
    metric_stds:
    - 0.021
    - null
  - model: CoMPT
    model_plain: CoMPT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.877
    - null
    metric_stds:
    - null
    - null
  - model: AttrMask
    model_plain: AttrMask
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.18407'
    title: A Group Symmetric Stochastic Differential Equation Model for Molecule Multi-modal
      Pretraining
    date: May 28, 2023
    date_iso: '2023-05-28'
    date_display: May 2023
    codebase_url: https://github.com/chao1224/MoleculeSDE
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.877
    - null
    metric_stds:
    - 0.0119
    - null
  - model: MoleBlend
    model_plain: MoleBlend
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.10343'
    title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view Molecular
      Representation Learning'
    date: May 15, 2024
    date_iso: '2024-05-15'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.876
    - null
    metric_stds:
    - 0.007
    - null
  - model: N-Gram_XGB
    model_plain: N-Gram_XGB
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.875
    - null
    metric_stds:
    - 0.027
    - null
  - model: GSAT
    model_plain: GSAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.15745'
    title: Robust Ante-hoc Graph Explainer using Bilevel Optimization
    date: May 25, 2023
    date_iso: '2023-05-25'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.875
    - null
    metric_stds:
    - 0.027
    - null
  - model: N-GramXGB
    model_plain: N-GramXGB
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.875
    - null
    metric_stds:
    - 0.027
    - null
  - model: MoleculeSDE
    model_plain: MoleculeSDE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.18407'
    title: A Group Symmetric Stochastic Differential Equation Model for Molecule Multi-modal
      Pretraining
    date: May 28, 2023
    date_iso: '2023-05-28'
    date_display: May 2023
    codebase_url: https://github.com/chao1224/MoleculeSDE
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.87
    - null
    metric_stds:
    - 0.0053
    - null
  - model: AGCN
    model_plain: AGCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '1801.03226'
    title: Adaptive Graph Convolutional Neural Networks
    date: Jan 10, 2018
    date_iso: '2018-01-10'
    date_display: Jan 2018
    codebase_url: ''
    published_conference: AAAI 2018
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2018
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8678
    - null
    metric_stds:
    - null
    - null
  - model: PNA
    model_plain: PNA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1.8
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.867
    - null
    metric_stds:
    - 0.011
    - null
  - model: GraphMVP
    model_plain: GraphMVP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.18407'
    title: A Group Symmetric Stochastic Differential Equation Model for Molecule Multi-modal
      Pretraining
    date: May 28, 2023
    date_iso: '2023-05-28'
    date_display: May 2023
    codebase_url: https://github.com/chao1224/MoleculeSDE
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.865
    - null
    metric_stds:
    - 0.017
    - null
  row_count: 315
  rows_json: /data/datasets/clintox/scaffold-split-rows.json
  chart_json: /data/datasets/clintox/scaffold-split-chart.json
  arch_counts:
    gnn: 189
    hybrid: 74
    graph_transformer: 6
    llm: 6
    walk: 1
    traditional: 20
  metric_counts:
  - 302
  - 13
  milestones: &id001
  - value: 0.8678
    std: null
    model: AGCN
    arxiv_id: '1801.03226'
    title: Adaptive Graph Convolutional Neural Networks
    date: '2018-01-10'
  - value: 0.906
    std: 0.006
    model: D-MPNN
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: '2021-06-11'
  - value: 0.919
    std: null
    model: GeomGCL
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: '2021-09-24'
  - value: 0.937
    std: null
    model: Molformer
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: '2021-10-04'
  - value: 0.954
    std: 0.011
    model: iMolCLR
    arxiv_id: '2202.09346'
    title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation
      and Decomposed Fragment Contrast
    date: '2022-02-18'
  - value: 0.983
    std: 0.017
    model: UniMAP
    arxiv_id: '2310.14216'
    title: 'UniMAP: Universal SMILES-Graph Representation Learning'
    date: '2023-10-22'
  - value: 0.993
    std: 0.004
    model: SE(3)-I MPPH
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: '2023-12-12'
  milestones_by_metric:
    ROC-AUC: *id001
    Accuracy:
    - value: 0.8598
      std: 0.0127
      model: LAMP-Soft
      arxiv_id: '2410.10365'
      title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without
        Positive Samples'
      date: '2024-10-14'
---

