---
title: Dual-perspective Cross Contrastive Learning in Graph Transformers
arxiv_id: '2406.00403'
source_url: ''
authors:
- name: Zelin Yao
  orcid: null
  s2_author_id: '2298560734'
  s2_url: null
- name: Chuang Liu
  orcid: null
  s2_author_id: '145760439'
  s2_url: null
- name: Xueqi Ma
  orcid: null
  s2_author_id: '2249043738'
  s2_url: null
- name: Mukun Chen
  orcid: null
  s2_author_id: '2108227988'
  s2_url: null
- name: Jia Wu
  orcid: null
  s2_author_id: '2248803714'
  s2_url: null
- name: Xiantao Cai
  orcid: null
  s2_author_id: '2274151429'
  s2_url: null
- name: Bo Du
  orcid: null
  s2_author_id: '2248204457'
  s2_url: null
- name: Wenbin Hu
  orcid: null
  s2_author_id: '2146226874'
  s2_url: null
published_date: Jun 1, 2024
published_date_iso: '2024-06-01'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph contrastive learning (GCL) is a popular method for leaning graph
  representations by maximizing the consistency of features across augmented views.
  Traditional GCL methods utilize single-perspective (i.e. data or model-perspective)
  augmentation to generate positive samples, restraining the diversity of positive
  samples. In addition, these positive samples may be unreliable due to uncontrollable
  augmentation strategies that potentially alter the semantic information. To address
  these challenges, this paper proposed a innovative framework termed dual-perspective
  cross graph contrastive learning (DC-GCL), which incorporates three modifications
  designed to enhance positive sample diversity and reliability: 1) We propose dual-perspective
  augmentation strategy that provide the model with more diverse training data, enabling
  the model effective learning of feature consistency across different views. 2) From
  the data perspective, we slightly perturb the original graphs using controllable
  data augmentation, effectively preserving their semantic information. 3) From the
  model perspective, we enhance the encoder by utilizing more powerful graph transformers
  instead of graph neural networks. Based on the model''s architecture, we propose
  three pruning-based strategies to slightly perturb the encoder, providing more reliable
  positive samples. These modifications collectively form the DC-GCL''s foundation
  and provide more diverse and reliable training inputs, offering significant improvements
  over traditional GCL methods. Extensive experiments on various benchmarks demonstrate
  that DC-GCL consistently outperforms different baselines on various datasets and
  tasks..'
codebase_url: https://github.com/Celin-Yao/DC-GCL
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DC-GCL
mrr: 0.0148
adjusted_mrr: 0.0148
mrr_dataset_count: 9
benchmark_categories:
- TU Dortmund
- MoleculeNet
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 6
  total: 11
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 3
  total: 9
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id007
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
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.773
    std: 0.005
    paper_value: 0.773
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
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
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
    gap_vs_at_pub: 0.06099999999999994
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
    value_gap: 0.06099999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.834
    sort_std: 0.033
    global_rank: 97
    paper_rank: 218
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
  - model: DC-GCL
    model_key: dc-gcl
    model_plain: DC-GCL
    value: 0.799
    std: 0.017
    paper_value: 0.799
    paper_std: 0.017
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.799
    true_std: 0.017
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.799
    sort_std: 0.017
    global_rank: 170
    paper_rank: 170
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ContextPred
    model_key: contextpred
    model_plain: ContextPred
    value: 0.796
    std: 0.012
    paper_value: 0.796
    paper_std: 0.012
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: pretraingnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.796
    at_pub_std: 0.012
    at_pub_source_arxiv: '2202.02989'
    at_pub_source_title: Graph Self-supervised Learning with Accurate Discrepancy
      Learning
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-06-16'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.796
    true_std: 0.012
    value_gap_source_arxiv: '2206.07869'
    value_gap_source_title: Let Invariant Rationale Discovery Inspire Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.796
    sort_std: 0.012
    global_rank: 177
    paper_rank: 177
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AttrMasking
    model_key: attrmasking
    model_plain: AttrMasking
    value: 0.793
    std: 0.016
    paper_value: 0.793
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: pretraingnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.793
    at_pub_std: 0.016
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-16'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.793
    true_std: 0.016
    value_gap_source_arxiv: '2206.07869'
    value_gap_source_title: Let Invariant Rationale Discovery Inspire Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.793
    sort_std: 0.016
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.754
    std: 0.014
    paper_value: 0.754
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
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: graphCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
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
    gap_vs_at_pub: 0.028000000000000025
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
    value_gap: 0.028000000000000025
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.012
    global_rank: 205
    paper_rank: 238
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    comparison_source_arxiv: '2205.15746'
    is_best: false
    is_std_outlier: false
  - model: DRGCL
    model_key: drgcl
    model_plain: DRGCL
    value: 0.782
    std: 0.01
    paper_value: 0.782
    paper_std: 0.01
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
    table_ref: Table 3
    source_ref: drgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.782
    true_std: 0.01
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.01
    global_rank: 206
    paper_rank: 206
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Infomax
    model_key: infomax
    model_plain: Infomax
    value: 0.759
    std: 0.016
    paper_value: 0.759
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: pretraingnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.759
    at_pub_std: 0.016
    at_pub_source_arxiv: '2202.02989'
    at_pub_source_title: Graph Self-supervised Learning with Accurate Discrepancy
      Learning
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.778
    true_std: 0.0046
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.019000000000000017
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.0046
    global_rank: 216
    paper_rank: 234
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: No-pretrain
    model_key: no-pretrain
    model_plain: No-pretrain
    value: 0.77
    std: 0.021
    paper_value: 0.77
    paper_std: 0.021
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7
    at_pub_std: 0.025
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07000000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.77
    true_std: 0.021
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.77
    sort_std: 0.021
    global_rank: 223
    paper_rank: 223
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    comparison_source_arxiv: '2205.10803'
    is_best: false
    is_std_outlier: false
  - model: RGCL
    model_key: rgcl
    model_plain: RGCL
    value: 0.76
    std: 0.008
    paper_value: 0.76
    paper_std: 0.008
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
    table_ref: Table 3
    source_ref: rgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7603
    at_pub_std: 0.0077
    at_pub_source_arxiv: '2206.07869'
    at_pub_source_title: Let Invariant Rationale Discovery Inspire Graph Contrastive
      Learning
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-06-16'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7603
    true_std: 0.0077
    value_gap_source_arxiv: '2206.07869'
    value_gap_source_title: Let Invariant Rationale Discovery Inspire Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.7603
    sort_std: 0.0077
    global_rank: 233
    paper_rank: 233
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimGRACE
    model_key: simgrace
    model_plain: SimGRACE
    value: 0.75
    std: 0.017
    paper_value: 0.75
    paper_std: 0.017
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
    table_ref: Table 3
    source_ref: simgrace
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.758
    at_pub_std: 0.004
    at_pub_source_arxiv: '2403.01400'
    at_pub_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    at_pub_source_date_iso: '2024-03-03'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-03'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.008000000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.758
    true_std: 0.004
    value_gap_source_arxiv: '2403.01400'
    value_gap_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    value_gap_source_is_current_paper: false
    value_gap: 0.008000000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.758
    sort_std: 0.004
    global_rank: 235
    paper_rank: 240
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ADGCL
    model_key: adgcl
    model_plain: ADGCL
    value: 0.74
    std: 0.022
    paper_value: 0.74
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
    table_ref: Table 3
    source_ref: adgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on BACE using Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.74
    at_pub_std: 0.022
    at_pub_source_arxiv: '2310.14753'
    at_pub_source_title: Rethinking Tokenizer and Decoder in Masked Graph Modeling
      for Molecules
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.74
    true_std: 0.022
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.74
    sort_std: 0.022
    global_rank: 245
    paper_rank: 245
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
  dataset: COLLAB
  rows:
  - model: GPM
    model_key: wl-mlp
    model_plain: GPM
    value: 0.9792
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
    sort_value: 0.9792
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: msh-gnn
    model_plain: GPM
    value: 0.964
    std: 0.007
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
    global_rank: 2
    sort_value: 0.964
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPM
    model_key: cocn
    model_plain: GPM
    value: 0.8722
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.18480'
    title: Scalable Graph Compressed Convolutions
    date: Jul 26, 2024
    date_display: Jul 2024
    date_iso: '2024-07-26'
    venue: arXiv.org
    codebase_url: https://github.com/sunjss/CoCN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: use the one-hot encoding of node degrees as node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.8722
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.6933
    std: 0.0034
    paper_value: 0.6933
    paper_std: 0.0034
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8216
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.12829999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8216
    true_std: 0.0017
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.12829999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8216
    sort_std: 0.0017
    global_rank: 40
    paper_rank: 338
    rank_delta: 298
    rank_delta_abs: 298
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: SimGRACE
    model_key: simgrace
    model_plain: SimGRACE
    value: 0.7172
    std: 0.0082
    paper_value: 0.7172
    paper_std: 0.0082
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
    source_ref: simgrace
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8188
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.10160000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8188
    true_std: 0.0023
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.10160000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8188
    sort_std: 0.0023
    global_rank: 44
    paper_rank: 318
    rank_delta: 274
    rank_delta_abs: 274
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.814
    std: 0.0026
    paper_value: 0.814
    paper_std: 0.0026
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.814
    true_std: 0.0026
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.814
    sort_std: 0.0026
    global_rank: 73
    paper_rank: 73
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.7136
    std: 0.0115
    paper_value: 0.7136
    paper_std: 0.0115
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
    source_ref: graphCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8108
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.09719999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8108
    true_std: 0.0017
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.09719999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8108
    sort_std: 0.0017
    global_rank: 92
    paper_rank: 322
    rank_delta: 230
    rank_delta_abs: 230
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: DC-GCL
    model_key: dc-gcl
    model_plain: DC-GCL
    value: 0.7983
    std: 0.0043
    paper_value: 0.7983
    paper_std: 0.0043
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7983
    true_std: 0.0043
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7983
    sort_std: 0.0043
    global_rank: 150
    paper_rank: 150
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphTrans
    model_key: graphtrans
    model_plain: GraphTrans
    value: 0.7981
    std: 0.0084
    paper_value: 0.7981
    paper_std: 0.0084
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphtrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7981
    at_pub_std: 0.0084
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7981
    true_std: 0.0084
    value_gap_source_arxiv: '2310.11025'
    value_gap_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7981
    sort_std: 0.0084
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
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.7065
    std: 0.0113
    paper_value: 0.7065
    paper_std: 0.0113
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
    source_ref: infoGraph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.794
    at_pub_std: null
    at_pub_source_arxiv: '2103.00959'
    at_pub_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    at_pub_source_date_iso: '2021-03-01'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2021-03-01'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.08750000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.794
    true_std: null
    value_gap_source_arxiv: '2103.00959'
    value_gap_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.08750000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.794
    sort_std: null
    global_rank: 165
    paper_rank: 328
    rank_delta: 163
    rank_delta_abs: 163
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    comparison_source_arxiv: '2103.00959'
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.695
    std: 0.0036
    paper_value: 0.695
    paper_std: 0.0036
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7535
    at_pub_std: 0.0093
    at_pub_source_arxiv: '2210.00643'
    at_pub_source_title: Spectral Augmentation for Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-06-04'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.058499999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7553
    true_std: 0.0018
    value_gap_source_arxiv: '2406.01899'
    value_gap_source_title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion
      Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.06030000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7553
    sort_std: 0.0018
    global_rank: 268
    paper_rank: 338
    rank_delta: 70
    rank_delta_abs: 70
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Augmentation for Self-Supervised Learning on
      Graphs
    comparison_source_arxiv: '2210.00643'
    is_best: false
    is_std_outlier: false
  - model: DualGCL
    model_key: dualgcl
    model_plain: DualGCL
    value: 0.753
    std: 0.004
    paper_value: 0.753
    paper_std: 0.004
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
    source_ref: dualgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.753
    true_std: 0.004
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.753
    sort_std: 0.004
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
  - model: iGCL
    model_key: igcl
    model_plain: iGCL
    value: 0.72
    std: 0.008
    paper_value: 0.72
    paper_std: 0.008
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
    source_ref: igcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.72
    true_std: 0.008
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.72
    sort_std: 0.008
    global_rank: 316
    paper_rank: 316
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRGCL
    model_key: drgcl
    model_plain: DRGCL
    value: 0.706
    std: 0.008
    paper_value: 0.706
    paper_std: 0.008
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
    source_ref: drgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on COLLAB dataset using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.706
    true_std: 0.008
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.706
    sort_std: 0.008
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id008
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
  - model: RGCL
    model_key: rgcl
    model_plain: RGCL
    value: 0.764
    std: 0.034
    paper_value: 0.764
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: rgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.85
    at_pub_std: 0.008
    at_pub_source_arxiv: '2310.14753'
    at_pub_source_title: Rethinking Tokenizer and Decoder in Masked Graph Modeling
      for Molecules
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-06-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.08599999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.834
    true_std: 0.009
    value_gap_source_arxiv: '2306.03506'
    value_gap_source_title: Subgraph Networks Based Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.06999999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.834
    sort_std: 0.009
    global_rank: 62
    paper_rank: 115
    rank_delta: 53
    rank_delta_abs: 53
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Rethinking Tokenizer and Decoder in Masked Graph Modeling
      for Molecules
    comparison_source_arxiv: '2310.14753'
    is_best: false
    is_std_outlier: false
  - model: DC-GCL
    model_key: dc-gcl
    model_plain: DC-GCL
    value: 0.827
    std: 0.036
    paper_value: 0.827
    paper_std: 0.036
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: unknown
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.827
    true_std: 0.036
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.827
    sort_std: 0.036
    global_rank: 63
    paper_rank: 63
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
    value: 0.813
    std: 0.025
    paper_value: 0.813
    paper_std: 0.025
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8132
    at_pub_std: 0.0249
    at_pub_source_arxiv: '2202.02989'
    at_pub_source_title: Graph Self-supervised Learning with Accurate Discrepancy
      Learning
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-02-07'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.000200000000000089
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8132
    true_std: 0.0249
    value_gap_source_arxiv: '2202.02989'
    value_gap_source_title: Graph Self-supervised Learning with Accurate Discrepancy
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.000200000000000089
    has_value_note: false
    value_note: ''
    sort_value: 0.8132
    sort_std: 0.0249
    global_rank: 77
    paper_rank: 77
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ADGCL
    model_key: adgcl
    model_plain: ADGCL
    value: 0.785
    std: 0.037
    paper_value: 0.785
    paper_std: 0.037
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: adgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.798
    at_pub_std: 0.035
    at_pub_source_arxiv: '2306.03506'
    at_pub_source_title: Subgraph Networks Based Contrastive Learning
    at_pub_source_date_iso: '2023-06-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.013000000000000012
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.798
    true_std: 0.035
    value_gap_source_arxiv: '2306.03506'
    value_gap_source_title: Subgraph Networks Based Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.013000000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.798
    sort_std: 0.035
    global_rank: 90
    paper_rank: 101
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.76
    std: 0.027
    paper_value: 0.76
    paper_std: 0.027
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: graphCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.789
    at_pub_std: 0.042
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.029000000000000026
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.789
    true_std: 0.042
    value_gap_source_arxiv: '2110.07728'
    value_gap_source_title: 16 Pre-training Molecular Graph Representation with 3D
      Geometry
    value_gap_source_is_current_paper: false
    value_gap: 0.029000000000000026
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.042
    global_rank: 94
    paper_rank: 117
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRGCL
    model_key: drgcl
    model_plain: DRGCL
    value: 0.782
    std: 0.015
    paper_value: 0.782
    paper_std: 0.015
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: drgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.782
    true_std: 0.015
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.015
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
  - model: ContextPred
    model_key: contextpred
    model_plain: ContextPred
    value: 0.659
    std: 0.038
    paper_value: 0.659
    paper_std: 0.038
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: pretraingnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.772
    at_pub_std: 0.0088
    at_pub_source_arxiv: '2305.18407'
    at_pub_source_title: A Group Symmetric Stochastic Differential Equation Model
      for Molecule Multi-modal Pretraining
    at_pub_source_date_iso: '2023-05-28'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-09'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.11299999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.772
    true_std: 0.0088
    value_gap_source_arxiv: '2405.05665'
    value_gap_source_title: 'SubGDiff: A Subgraph Diffusion Model to Improve Molecular
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.11299999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.772
    sort_std: 0.0088
    global_rank: 112
    paper_rank: 196
    rank_delta: 84
    rank_delta_abs: 84
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Group Symmetric Stochastic Differential Equation Model
      for Molecule Multi-modal Pretraining
    comparison_source_arxiv: '2305.18407'
    is_best: false
    is_std_outlier: false
  - model: SimGRACE
    model_key: simgrace
    model_plain: SimGRACE
    value: 0.756
    std: 0.03
    paper_value: 0.756
    paper_std: 0.03
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: simgrace
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.668
    at_pub_std: 0.02
    at_pub_source_arxiv: '2403.01400'
    at_pub_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    at_pub_source_date_iso: '2024-03-03'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08799999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.756
    true_std: 0.03
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.756
    sort_std: 0.03
    global_rank: 120
    paper_rank: 120
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    comparison_source_arxiv: '2403.01400'
    is_best: false
    is_std_outlier: false
  - model: Infomax
    model_key: infomax
    model_plain: Infomax
    value: 0.699
    std: 0.03
    paper_value: 0.699
    paper_std: 0.03
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: pretraingnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.73
    at_pub_std: 0.032
    at_pub_source_arxiv: '2110.00987'
    at_pub_source_title: Motif-based Graph Self-Supervised Learning for Molecular
      Property Prediction
    at_pub_source_date_iso: '2021-10-03'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2021-10-03'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.031000000000000028
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.73
    true_std: 0.032
    value_gap_source_arxiv: '2110.00987'
    value_gap_source_title: Motif-based Graph Self-Supervised Learning for Molecular
      Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.031000000000000028
    has_value_note: false
    value_note: ''
    sort_value: 0.73
    sort_std: 0.032
    global_rank: 148
    paper_rank: 173
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AttrMasking
    model_key: attrmasking
    model_plain: AttrMasking
    value: 0.718
    std: 0.041
    paper_value: 0.718
    paper_std: 0.041
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
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: pretraingnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.718
    at_pub_std: 0.041
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-16'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.718
    true_std: 0.041
    value_gap_source_arxiv: '2206.07869'
    value_gap_source_title: Let Invariant Rationale Discovery Inspire Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.718
    sort_std: 0.041
    global_rank: 160
    paper_rank: 160
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: No-pretrain
    model_key: no-pretrain
    model_plain: No-pretrain
    value: 0.644
    std: 0.042
    paper_value: 0.644
    paper_std: 0.042
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on ClinTox using Scaffold split (transfer learning setup)
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.582
    at_pub_std: 0.028
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.062000000000000055
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.644
    true_std: 0.042
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.644
    sort_std: 0.042
    global_rank: 204
    paper_rank: 204
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
- &id005
  dataset: D&D
  rows:
  - model: ECC
    model_key: gc-gnn (graphsage)
    model_plain: ECC
    value: 0.921
    std: 0.081
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.00738'
    title: Rethinking the Power of Graph Canonization in Graph Representation Learning
      with Stability
    date: Sep 1, 2023
    date_display: Sep 2023
    date_iso: '2023-09-01'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.921
    sort_std: 0.081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: sugar
    model_plain: ECC
    value: 0.8403
    std: 0.0133
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2101.08170'
    title: 'SUGAR: Subgraph Neural Network with Reinforcement Pooling and Self-Supervised
      Mutual Information Mechanism'
    date: Jan 20, 2021
    date_display: Jan 2021
    date_iso: '2021-01-20'
    venue: The Web Conference
    codebase_url: https://github.com/RingBDStack/SUGAR
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8403
    sort_std: 0.0133
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: ortho-g-u-nets
    model_plain: ECC
    value: 0.8387
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2109.11338'
    title: Orthogonal Graph Neural Networks
    date: Sep 23, 2021
    date_display: Sep 2021
    date_iso: '2021-09-23'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8387
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DC-GCL
    model_key: dc-gcl
    model_plain: DC-GCL
    value: 0.7943
    std: 0.0063
    paper_value: 0.7943
    paper_std: 0.0063
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: DC-GCL incorporates a comprehensive version of data and
      model augmentation... we generate an increased number of correlated views within
      the DC-GCL framework.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on D&D for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7943
    true_std: 0.0063
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7943
    sort_std: 0.0063
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.7862
    std: 0.004
    paper_value: 0.7862
    paper_std: 0.004
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
    source_ref: graphCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on D&D for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7862
    true_std: 0.004
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7862
    sort_std: 0.004
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
  - model: DRGCL
    model_key: drgcl
    model_plain: DRGCL
    value: 0.784
    std: 0.007
    paper_value: 0.784
    paper_std: 0.007
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
    source_ref: drgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on D&D for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.784
    true_std: 0.007
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.784
    sort_std: 0.007
    global_rank: 71
    paper_rank: 71
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimGRACE
    model_key: simgrace
    model_plain: SimGRACE
    value: 0.7744
    std: 0.0111
    paper_value: 0.7744
    paper_std: 0.0111
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
    source_ref: simgrace
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on D&D for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7744
    true_std: 0.0111
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7744
    sort_std: 0.0111
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
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.774
    std: 0.0115
    paper_value: 0.774
    paper_std: 0.0115
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on D&D for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.774
    true_std: 0.0115
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.774
    sort_std: 0.0115
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
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.7732
    std: 0.0054
    paper_value: 0.7732
    paper_std: 0.0054
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on D&D for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7732
    true_std: 0.0054
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7732
    sort_std: 0.0054
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
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.7598
    std: 0.0153
    paper_value: 0.7598
    paper_std: 0.0153
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on D&D for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7598
    true_std: 0.0153
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7598
    sort_std: 0.0153
    global_rank: 128
    paper_rank: 128
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphTrans
    model_key: graphtrans
    model_plain: GraphTrans
    value: 0.7524
    std: 0.0483
    paper_value: 0.7524
    paper_std: 0.0483
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphtrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on D&D for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7524
    true_std: 0.0483
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7524
    sort_std: 0.0483
    global_rank: 144
    paper_rank: 144
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.7285
    std: 0.0178
    paper_value: 0.7285
    paper_std: 0.0178
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
    source_ref: infoGraph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on D&D for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7424
    at_pub_std: 0.0086
    at_pub_source_arxiv: '2009.05923'
    at_pub_source_title: Contrastive Self-supervised Learning for Graph Classification
    at_pub_source_date_iso: '2020-09-13'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.013899999999999912
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7424
    true_std: 0.0086
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.013899999999999912
    has_value_note: false
    value_note: ''
    sort_value: 0.7424
    sort_std: 0.0086
    global_rank: 158
    paper_rank: 166
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
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
  - model: DC-GCL
    model_key: dc-gcl
    model_plain: DC-GCL
    value: 0.905
    std: 0.0155
    paper_value: 0.905
    paper_std: 0.0155
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: DC-GCL incorporates a comprehensive version of data and
      model augmentation... uses GTs as encoders.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.905
    true_std: 0.0155
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.905
    sort_std: 0.0155
    global_rank: 136
    paper_rank: 136
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.8072
    std: 0.03
    paper_value: 0.8072
    paper_std: 0.03
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
    source_ref: wl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.904
    at_pub_std: 0.057
    at_pub_source_arxiv: '1912.06058'
    at_pub_source_title: Coloring graph neural networks for node disambiguation
    at_pub_source_date_iso: '2019-12-12'
    at_pub_source_date_label: IJCAI 2019
    value_gap_source_date_iso: '2022-05-26'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.0968
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
    value_gap: 0.0968
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.057
    global_rank: 141
    paper_rank: 603
    rank_delta: 462
    rank_delta_abs: 462
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Coloring graph neural networks for node disambiguation
    comparison_source_arxiv: '1912.06058'
    is_best: false
    is_std_outlier: false
  - model: iGCL
    model_key: igcl
    model_plain: iGCL
    value: 0.898
    std: 0.012
    paper_value: 0.898
    paper_std: 0.012
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
    source_ref: igcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.898
    true_std: 0.012
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.898
    sort_std: 0.012
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
  - model: DRGCL
    model_key: drgcl
    model_plain: DRGCL
    value: 0.895
    std: 0.006
    paper_value: 0.895
    paper_std: 0.006
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
    source_ref: drgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.895
    true_std: 0.006
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.895
    sort_std: 0.006
    global_rank: 210
    paper_rank: 210
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.8901
    std: 0.0113
    paper_value: 0.8901
    paper_std: 0.0113
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
    source_ref: infoGraph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.893
    at_pub_std: 0.0514
    at_pub_source_arxiv: '2305.19903'
    at_pub_source_title: Improving Expressivity of GNNs with Subgraph-specific Factor
      Embedded Normalization
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.0029000000000000137
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.893
    true_std: 0.0514
    value_gap_source_arxiv: '2305.19903'
    value_gap_source_title: Improving Expressivity of GNNs with Subgraph-specific
      Factor Embedded Normalization
    value_gap_source_is_current_paper: false
    value_gap: 0.0029000000000000137
    has_value_note: false
    value_note: ''
    sort_value: 0.893
    sort_std: 0.0514
    global_rank: 236
    paper_rank: 251
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimGRACE
    model_key: simgrace
    model_plain: SimGRACE
    value: 0.8901
    std: 0.0131
    paper_value: 0.8901
    paper_std: 0.0131
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
    source_ref: simgrace
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.891
    at_pub_std: 0.014
    at_pub_source_arxiv: '2401.16011'
    at_pub_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    at_pub_source_date_iso: '2024-01-29'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-01-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0009000000000000119
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.891
    true_std: 0.014
    value_gap_source_arxiv: '2401.16011'
    value_gap_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    value_gap_source_is_current_paper: false
    value_gap: 0.0009000000000000119
    has_value_note: false
    value_note: ''
    sort_value: 0.891
    sort_std: 0.014
    global_rank: 251
    paper_rank: 251
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DualGCL
    model_key: dualgcl
    model_plain: DualGCL
    value: 0.885
    std: 0.009
    paper_value: 0.885
    paper_std: 0.009
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
    source_ref: dualgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.885
    true_std: 0.009
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.885
    sort_std: 0.009
    global_rank: 289
    paper_rank: 289
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.868
    std: 0.0134
    paper_value: 0.868
    paper_std: 0.0134
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
    source_ref: graphCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8829
    at_pub_std: 0.0131
    at_pub_source_arxiv: '2309.16014'
    at_pub_source_title: Graph-level Representation Learning with Joint-Embedding
      Predictive Architectures
    at_pub_source_date_iso: '2023-09-27'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-09-27'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.014900000000000024
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8829
    true_std: 0.0131
    value_gap_source_arxiv: '2309.16014'
    value_gap_source_title: Graph-level Representation Learning with Joint-Embedding
      Predictive Architectures
    value_gap_source_is_current_paper: false
    value_gap: 0.014900000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.8829
    sort_std: 0.0131
    global_rank: 301
    paper_rank: 377
    rank_delta: 76
    rank_delta_abs: 76
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.8735
    std: 0.0102
    paper_value: 0.8735
    paper_std: 0.0102
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.877
    at_pub_std: null
    at_pub_source_arxiv: '2103.00111'
    at_pub_source_title: 'Graph Self-Supervised Learning: A Survey'
    at_pub_source_date_iso: '2021-02-27'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-02-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.0034999999999999476
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.877
    true_std: null
    value_gap_source_arxiv: '2103.00111'
    value_gap_source_title: 'Graph Self-Supervised Learning: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.0034999999999999476
    has_value_note: false
    value_note: ''
    sort_value: 0.877
    sort_std: null
    global_rank: 327
    paper_rank: 346
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.8767
    std: 0.0079
    paper_value: 0.8767
    paper_std: 0.0079
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8967
    at_pub_std: 0.0524
    at_pub_source_arxiv: '2401.03638'
    at_pub_source_title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    at_pub_source_date_iso: '2024-01-08'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2021-06-10'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8767
    true_std: 0.0079
    value_gap_source_arxiv: '2106.05819'
    value_gap_source_title: Adversarial Graph Augmentation to Improve Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8767
    sort_std: 0.0079
    global_rank: 331
    paper_rank: 331
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.8744
    std: 0.0272
    paper_value: 0.8744
    paper_std: 0.0272
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: dgk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8744
    at_pub_std: 0.027
    at_pub_source_arxiv: '1905.11136'
    at_pub_source_title: Provably Powerful Graph Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8744
    true_std: 0.0272
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8744
    sort_std: 0.0272
    global_rank: 339
    paper_rank: 339
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphTrans
    model_key: graphtrans
    model_plain: GraphTrans
    value: 0.8722
    std: 0.0705
    paper_value: 0.8722
    paper_std: 0.0705
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphtrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8154
    at_pub_std: 0.0091
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05679999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8722
    true_std: 0.0705
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8722
    sort_std: 0.0705
    global_rank: 356
    paper_rank: 356
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GL
    model_key: gl
    model_plain: GL
    value: 0.8166
    std: 0.0211
    paper_value: 0.8166
    paper_std: 0.0211
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
    source_ref: gl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.852
    at_pub_std: 0.009
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2016-06-03'
    value_gap_source_date_label: NeurIPS 2016
    gap_vs_at_pub: 0.03539999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.852
    true_std: 0.009
    value_gap_source_arxiv: '1606.01141'
    value_gap_source_title: On Valid Optimal Assignment Kernels and Applications to
      Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.03539999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.852
    sort_std: 0.009
    global_rank: 434
    paper_rank: 583
    rank_delta: 149
    rank_delta_abs: 149
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Valid Optimal Assignment Kernels and Applications
      to Graph Classification
    comparison_source_arxiv: '1606.01141'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.85
    std: 0.0316
    paper_value: 0.85
    paper_std: 0.0316
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.85
    true_std: 0.0316
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.85
    sort_std: 0.0316
    global_rank: 438
    paper_rank: 438
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
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.8001
    std: 0.005
    paper_value: 0.8001
    paper_std: 0.005
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
    source_ref: wl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86
    at_pub_std: 0.018
    at_pub_source_arxiv: '2205.14368'
    at_pub_source_title: Going Deeper into Permutation-Sensitive Graph Neural Networks
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.05989999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.86
    true_std: 0.018
    value_gap_source_arxiv: '2205.14368'
    value_gap_source_title: Going Deeper into Permutation-Sensitive Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.05989999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.018
    global_rank: 10
    paper_rank: 226
    rank_delta: 216
    rank_delta_abs: 216
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Going Deeper into Permutation-Sensitive Graph Neural
      Networks
    comparison_source_arxiv: '2205.14368'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.8421
    std: 0.0225
    paper_value: 0.8421
    paper_std: 0.0225
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8421
    true_std: 0.0225
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8421
    sort_std: 0.0225
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
  - model: iGCL
    model_key: igcl
    model_plain: iGCL
    value: 0.827
    std: 0.004
    paper_value: 0.827
    paper_std: 0.004
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
    source_ref: igcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.827
    true_std: 0.004
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.827
    sort_std: 0.004
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
  - model: GraphTrans
    model_key: graphtrans
    model_plain: GraphTrans
    value: 0.826
    std: 0.012
    paper_value: 0.826
    paper_std: 0.012
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphtrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.826
    at_pub_std: 0.012
    at_pub_source_arxiv: '2201.08821'
    at_pub_source_title: Representing Long-Range Context for Graph Neural Networks
      with Global Attention
    at_pub_source_date_iso: '2022-01-21'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.826
    true_std: 0.012
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.826
    sort_std: 0.012
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.7787
    std: 0.0041
    paper_value: 0.7787
    paper_std: 0.0041
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
    source_ref: graphCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.825
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.04630000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.825
    true_std: 0.0013
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.04630000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.825
    sort_std: 0.0013
    global_rank: 104
    paper_rank: 342
    rank_delta: 238
    rank_delta_abs: 238
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: SimGRACE
    model_key: simgrace
    model_plain: SimGRACE
    value: 0.7912
    std: 0.0044
    paper_value: 0.7912
    paper_std: 0.0044
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
    source_ref: simgrace
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.818
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.026799999999999935
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.818
    true_std: 0.0015
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.026799999999999935
    has_value_note: false
    value_note: ''
    sort_value: 0.818
    sort_std: 0.0015
    global_rank: 138
    paper_rank: 267
    rank_delta: 129
    rank_delta_abs: 129
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.7836
    std: 0.0053
    paper_value: 0.7836
    paper_std: 0.0053
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.817
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.033399999999999985
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.817
    true_std: 0.0026
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.033399999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.817
    sort_std: 0.0026
    global_rank: 144
    paper_rank: 314
    rank_delta: 170
    rank_delta_abs: 170
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.8031
    std: 0.0046
    paper_value: 0.8031
    paper_std: 0.0046
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: dgk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8031
    at_pub_std: 0.0046
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8031
    true_std: 0.0046
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8031
    sort_std: 0.0046
    global_rank: 210
    paper_rank: 210
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DualGCL
    model_key: dualgcl
    model_plain: DualGCL
    value: 0.798
    std: 0.003
    paper_value: 0.798
    paper_std: 0.003
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
    source_ref: dualgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.798
    true_std: 0.003
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.798
    sort_std: 0.003
    global_rank: 239
    paper_rank: 239
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DC-GCL
    model_key: dc-gcl
    model_plain: DC-GCL
    value: 0.7962
    std: 0.0037
    paper_value: 0.7962
    paper_std: 0.0037
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: DC-GCL incorporates a comprehensive version of data and
      model augmentation... uses GTs as encoders
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7962
    true_std: 0.0037
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7962
    sort_std: 0.0037
    global_rank: 248
    paper_rank: 248
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRGCL
    model_key: drgcl
    model_plain: DRGCL
    value: 0.787
    std: 0.004
    paper_value: 0.787
    paper_std: 0.004
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
    source_ref: drgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.787
    true_std: 0.004
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.787
    sort_std: 0.004
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
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.7807
    std: 0.0047
    paper_value: 0.7807
    paper_std: 0.0047
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.784
    at_pub_std: 0.005
    at_pub_source_arxiv: '2205.15746'
    at_pub_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    at_pub_source_date_iso: '2022-05-31'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.0033000000000000806
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.784
    true_std: 0.005
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0033000000000000806
    has_value_note: false
    value_note: ''
    sort_value: 0.784
    sort_std: 0.005
    global_rank: 313
    paper_rank: 328
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.762
    std: 0.0106
    paper_value: 0.762
    paper_std: 0.0106
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
    source_ref: infoGraph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on NCI1 for graph classification
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.775
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.013000000000000012
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.775
    true_std: 0.0074
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.013000000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.775
    sort_std: 0.0074
    global_rank: 358
    paper_rank: 406
    rank_delta: 48
    rank_delta_abs: 48
    rank_delta_direction: worse
    has_value_gap: true
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
  dataset: PROTEINS
  rows:
  - model: Graphormer-SPIS
    model_key: gmn
    model_plain: Graphormer-SPIS
    value: 0.8225
    std: null
    metric: Accuracy
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
    global_rank: 1
    sort_value: 0.8225
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: ci-gnn
    model_plain: Graphormer-SPIS
    value: 0.82
    std: 0.02
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2301.01642'
    title: 'CI-GNN: A Granger Causality-Inspired Graph Neural Network for Interpretable
      Brain Network-Based Psychiatric Diagnosis'
    date: Jan 4, 2023
    date_display: Jan 2023
    date_iso: '2023-01-04'
    venue: Neural Networks
    codebase_url: https://github.com/ZKZ-Brain/CI-GNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.82
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: diffpool+gpl
    model_plain: Graphormer-SPIS
    value: 0.8196
    std: 0.0286
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.11361'
    title: 'Graph Structure Prompt Learning: A Novel Methodology to Improve Performance
      of Graph Neural Networks'
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    venue: Applied intelligence (Boston)
    codebase_url: https://github.com/PreckLi/graph_prompt_learning
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8196
    sort_std: 0.0286
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DC-GCL
    model_key: dc-gcl
    model_plain: DC-GCL
    value: 0.7645
    std: 0.0026
    paper_value: 0.7645
    paper_std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: DC-GCL incorporates a comprehensive version of data and
      model augmentation... uses GTs as encoders
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7645
    true_std: 0.0026
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7645
    sort_std: 0.0026
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.7577
    std: 0.0219
    paper_value: 0.7577
    paper_std: 0.0219
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7577
    true_std: 0.0219
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7577
    sort_std: 0.0219
    global_rank: 177
    paper_rank: 177
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.733
    std: 0.0082
    paper_value: 0.733
    paper_std: 0.0082
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: dgk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7568
    at_pub_std: 0.0255
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.023800000000000043
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7568
    true_std: 0.005
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: 0.023800000000000043
    has_value_note: false
    value_note: ''
    sort_value: 0.7568
    sort_std: 0.005
    global_rank: 187
    paper_rank: 360
    rank_delta: 173
    rank_delta_abs: 173
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.7292
    std: 0.0056
    paper_value: 0.7292
    paper_std: 0.0056
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
    source_ref: wl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.756
    at_pub_std: 0.004
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2016-06-03'
    value_gap_source_date_label: NeurIPS 2016
    gap_vs_at_pub: 0.026800000000000046
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.756
    true_std: 0.004
    value_gap_source_arxiv: '1606.01141'
    value_gap_source_title: On Valid Optimal Assignment Kernels and Applications to
      Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.026800000000000046
    has_value_note: false
    value_note: ''
    sort_value: 0.756
    sort_std: 0.004
    global_rank: 192
    paper_rank: 379
    rank_delta: 187
    rank_delta_abs: 187
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Valid Optimal Assignment Kernels and Applications
      to Graph Classification
    comparison_source_arxiv: '1606.01141'
    is_best: false
    is_std_outlier: false
  - model: DualGCL
    model_key: dualgcl
    model_plain: DualGCL
    value: 0.756
    std: 0.005
    paper_value: 0.756
    paper_std: 0.005
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
    source_ref: dualgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.756
    true_std: 0.005
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.756
    sort_std: 0.005
    global_rank: 197
    paper_rank: 197
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimGRACE
    model_key: simgrace
    model_plain: SimGRACE
    value: 0.7535
    std: 0.0009
    paper_value: 0.7535
    paper_std: 0.0009
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
    source_ref: simgrace
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7535
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2202.03104'
    at_pub_source_title: 'SimGRACE: A Simple Framework for Graph Contrastive Learning
      without Data Augmentation'
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2025-11-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7535
    true_std: 0.0009
    value_gap_source_arxiv: '2511.06216'
    value_gap_source_title: Adaptive Multi-view Graph Contrastive Learning via Fractional-order
      Neural Diffusion Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7535
    sort_std: 0.0009
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
  - model: DRGCL
    model_key: drgcl
    model_plain: DRGCL
    value: 0.752
    std: 0.006
    paper_value: 0.752
    paper_std: 0.006
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
    source_ref: drgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.752
    true_std: 0.006
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.752
    sort_std: 0.006
    global_rank: 238
    paper_rank: 238
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphTrans
    model_key: graphtrans
    model_plain: GraphTrans
    value: 0.7518
    std: 0.0336
    paper_value: 0.7518
    paper_std: 0.0336
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphtrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7512
    at_pub_std: 0.0489
    at_pub_source_arxiv: '2302.08671'
    at_pub_source_title: Search to Capture Long-range Dependency with Stacking GNNs
      for Graph Classification
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0006000000000000449
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7518
    true_std: 0.0336
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7518
    sort_std: 0.0336
    global_rank: 244
    paper_rank: 244
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.7439
    std: 0.0045
    paper_value: 0.7439
    paper_std: 0.0045
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
    source_ref: graphCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7489
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7489
    true_std: 0.0065
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0050000000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.7489
    sort_std: 0.0065
    global_rank: 275
    paper_rank: 309
    rank_delta: 34
    rank_delta_abs: 34
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: iGCL
    model_key: igcl
    model_plain: iGCL
    value: 0.748
    std: 0.005
    paper_value: 0.748
    paper_std: 0.005
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
    source_ref: igcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.748
    true_std: 0.005
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.748
    sort_std: 0.005
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
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.7455
    std: 0.0041
    paper_value: 0.7455
    paper_std: 0.0041
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.746
    at_pub_std: 0.004
    at_pub_source_arxiv: '2401.16011'
    at_pub_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    at_pub_source_date_iso: '2024-01-29'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.0004999999999999449
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.746
    true_std: 0.004
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.0004999999999999449
    has_value_note: false
    value_note: ''
    sort_value: 0.746
    sort_std: 0.004
    global_rank: 291
    paper_rank: 297
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.7444
    std: 0.0031
    paper_value: 0.7444
    paper_std: 0.0031
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
    source_ref: infoGraph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7444
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2202.03104'
    at_pub_source_title: 'SimGRACE: A Simple Framework for Graph Contrastive Learning
      without Data Augmentation'
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7444
    true_std: 0.0031
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7444
    sort_std: 0.0031
    global_rank: 306
    paper_rank: 306
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.7407
    std: 0.011
    paper_value: 0.7407
    paper_std: 0.011
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on PROTEINS dataset
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7407
    at_pub_std: 0.011
    at_pub_source_arxiv: '2202.03104'
    at_pub_source_title: 'SimGRACE: A Simple Framework for Graph Contrastive Learning
      without Data Augmentation'
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7407
    true_std: 0.011
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7407
    sort_std: 0.011
    global_rank: 321
    paper_rank: 321
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
- &id006
  dataset: RDT-B
  rows:
  - model: CIN
    model_key: oepg
    model_plain: CIN
    value: 0.963
    std: 0.009
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15746'
    title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
      Learning
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.963
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CIN
    model_key: msh-gnn
    model_plain: CIN
    value: 0.958
    std: 0.009
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
    global_rank: 2
    sort_value: 0.958
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CIN
    model_key: gnn-ak+
    model_plain: CIN
    value: 0.948
    std: 0.008
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.948
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DC-GCL
    model_key: dc-gcl
    model_plain: DC-GCL
    value: 0.9104
    std: 0.0045
    paper_value: 0.9104
    paper_std: 0.0045
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: DC-GCL incorporates a comprehensive version of data and
      model augmentation... uses GTs as encoders
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9104
    true_std: 0.0045
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9104
    sort_std: 0.0045
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
  - model: DRGCL
    model_key: drgcl
    model_plain: DRGCL
    value: 0.908
    std: 0.003
    paper_value: 0.908
    paper_std: 0.003
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
    source_ref: drgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.908
    true_std: 0.003
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.908
    sort_std: 0.003
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.8953
    std: 0.0084
    paper_value: 0.8953
    paper_std: 0.0084
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
    source_ref: graphCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9169
    at_pub_std: 0.007
    at_pub_source_arxiv: '2401.17580'
    at_pub_source_title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    at_pub_source_date_iso: '2024-01-31'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2022-06-16'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.021600000000000064
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8953
    true_std: 0.0084
    value_gap_source_arxiv: '2206.07869'
    value_gap_source_title: Let Invariant Rationale Discovery Inspire Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8953
    sort_std: 0.0084
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    comparison_source_arxiv: '2401.17580'
    is_best: false
    is_std_outlier: false
  - model: SimGRACE
    model_key: simgrace
    model_plain: SimGRACE
    value: 0.8951
    std: 0.0089
    paper_value: 0.8951
    paper_std: 0.0089
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
    source_ref: simgrace
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8951
    at_pub_std: 0.0089
    at_pub_source_arxiv: '2202.03104'
    at_pub_source_title: 'SimGRACE: A Simple Framework for Graph Contrastive Learning
      without Data Augmentation'
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2023-07-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8951
    true_std: 0.0089
    value_gap_source_arxiv: '2307.01053'
    value_gap_source_title: 'ENGAGE: Explanation Guided Data Augmentation for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8951
    sort_std: 0.0089
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.8642
    std: 0.0145
    paper_value: 0.8642
    paper_std: 0.0145
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8879
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2209.06560'
    at_pub_source_title: Graph Contrastive Learning with Personalized Augmentation
    at_pub_source_date_iso: '2022-09-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-09-14'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.023700000000000054
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8879
    true_std: 0.0065
    value_gap_source_arxiv: '2209.06560'
    value_gap_source_title: Graph Contrastive Learning with Personalized Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.023700000000000054
    has_value_note: false
    value_note: ''
    sort_value: 0.8879
    sort_std: 0.0065
    global_rank: 37
    paper_rank: 49
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Personalized Augmentation
    comparison_source_arxiv: '2209.06560'
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.825
    std: 0.0142
    paper_value: 0.825
    paper_std: 0.0142
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
    source_ref: infoGraph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8939
    at_pub_std: 0.0181
    at_pub_source_arxiv: '2401.17580'
    at_pub_source_title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    at_pub_source_date_iso: '2024-01-31'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2022-09-14'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06890000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8866
    true_std: 0.0095
    value_gap_source_arxiv: '2209.06560'
    value_gap_source_title: Graph Contrastive Learning with Personalized Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.0616000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8866
    sort_std: 0.0095
    global_rank: 38
    paper_rank: 57
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    comparison_source_arxiv: '2401.17580'
    is_best: false
    is_std_outlier: false
  - model: GraphTrans
    model_key: graphtrans
    model_plain: GraphTrans
    value: 0.8858
    std: 0.013
    paper_value: 0.8858
    paper_std: 0.013
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphtrans
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8858
    true_std: 0.013
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8858
    sort_std: 0.013
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
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.884
    std: 0.0115
    paper_value: 0.884
    paper_std: 0.0115
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.884
    true_std: 0.0115
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.884
    sort_std: 0.0115
    global_rank: 40
    paper_rank: 40
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
    value: 0.8529
    std: 0.0135
    paper_value: 0.8529
    paper_std: 0.0135
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
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9166
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2401.17580'
    at_pub_source_title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    at_pub_source_date_iso: '2024-01-31'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2022-09-14'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06369999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8814
    true_std: 0.0025
    value_gap_source_arxiv: '2209.06560'
    value_gap_source_title: Graph Contrastive Learning with Personalized Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.02849999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8814
    sort_std: 0.0025
    global_rank: 41
    paper_rank: 53
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    comparison_source_arxiv: '2401.17580'
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.7804
    std: 0.0039
    paper_value: 0.7804
    paper_std: 0.0039
    metric: Accuracy
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: dgk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7804
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2106.07594'
    at_pub_source_title: Graph Contrastive Learning Automated
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7804
    true_std: 0.0039
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7804
    sort_std: 0.0039
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
  - model: GL
    model_key: gl
    model_plain: GL
    value: 0.7734
    std: 0.0018
    paper_value: 0.7734
    paper_std: 0.0018
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
    source_ref: gl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7734
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2106.07594'
    at_pub_source_title: Graph Contrastive Learning Automated
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7734
    true_std: 0.0018
    value_gap_source_arxiv: '2506.06212'
    value_gap_source_title: Model-Driven Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7734
    sort_std: 0.0018
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
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.6882
    std: 0.0041
    paper_value: 0.6882
    paper_std: 0.0041
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
    source_ref: wl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on RDT-B using 10-fold CV
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6882
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2106.07594'
    at_pub_source_title: Graph Contrastive Learning Automated
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-07-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6882
    true_std: 0.0041
    value_gap_source_arxiv: '2307.01053'
    value_gap_source_title: 'ENGAGE: Explanation Guided Data Augmentation for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6882
    sort_std: 0.0041
    global_rank: 74
    paper_rank: 74
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
- &id009
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
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.6
    std: 0.008
    paper_value: 0.6
    paper_std: 0.008
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: joao
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.64
    at_pub_std: 0.01
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.040000000000000036
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.64
    true_std: 0.01
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.64
    sort_std: 0.01
    global_rank: 68
    paper_rank: 182
    rank_delta: 114
    rank_delta_abs: 114
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: ADGCL
    model_key: adgcl
    model_plain: ADGCL
    value: 0.591
    std: 0.009
    paper_value: 0.591
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: adgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.633
    at_pub_std: 0.008
    at_pub_source_arxiv: '2306.03506'
    at_pub_source_title: Subgraph Networks Based Contrastive Learning
    at_pub_source_date_iso: '2023-06-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.04200000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.633
    true_std: 0.008
    value_gap_source_arxiv: '2306.03506'
    value_gap_source_title: Subgraph Networks Based Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.04200000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.633
    sort_std: 0.008
    global_rank: 80
    paper_rank: 202
    rank_delta: 122
    rank_delta_abs: 122
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Subgraph Networks Based Contrastive Learning
    comparison_source_arxiv: '2306.03506'
    is_best: false
    is_std_outlier: false
  - model: ContextPred
    model_key: contextpred
    model_plain: ContextPred
    value: 0.609
    std: 0.006
    paper_value: 0.609
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: pretraingnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.622
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2305.18407'
    at_pub_source_title: A Group Symmetric Stochastic Differential Equation Model
      for Molecule Multi-modal Pretraining
    at_pub_source_date_iso: '2023-05-28'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-09'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.013000000000000012
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.622
    true_std: 0.0059
    value_gap_source_arxiv: '2405.05665'
    value_gap_source_title: 'SubGDiff: A Subgraph Diffusion Model to Improve Molecular
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.013000000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.622
    sort_std: 0.0059
    global_rank: 105
    paper_rank: 147
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Group Symmetric Stochastic Differential Equation Model
      for Molecule Multi-modal Pretraining
    comparison_source_arxiv: '2305.18407'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.605
    std: 0.009
    paper_value: 0.605
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: graphCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6176
    at_pub_std: 0.0111
    at_pub_source_arxiv: '2405.01350'
    at_pub_source_title: Community-Invariant Graph Contrastive Learning
    at_pub_source_date_iso: '2024-05-02'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.012600000000000056
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6183
    true_std: 0.006
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.013299999999999979
    has_value_note: false
    value_note: ''
    sort_value: 0.6183
    sort_std: 0.006
    global_rank: 116
    paper_rank: 163
    rank_delta: 47
    rank_delta_abs: 47
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Infomax
    model_key: infomax
    model_plain: Infomax
    value: 0.584
    std: 0.008
    paper_value: 0.584
    paper_std: 0.008
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: pretraingnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.616
    at_pub_std: 0.024
    at_pub_source_arxiv: '2206.03364'
    at_pub_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    at_pub_source_date_iso: '2022-06-02'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-02'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.03200000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.616
    true_std: 0.024
    value_gap_source_arxiv: '2206.03364'
    value_gap_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.03200000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.616
    sort_std: 0.024
    global_rank: 122
    paper_rank: 207
    rank_delta: 85
    rank_delta_abs: 85
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer
      for Molecular Property Prediction'
    comparison_source_arxiv: '2206.03364'
    is_best: false
    is_std_outlier: false
  - model: RGCL
    model_key: rgcl
    model_plain: RGCL
    value: 0.614
    std: 0.006
    paper_value: 0.614
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: rgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.614
    at_pub_std: 0.006
    at_pub_source_arxiv: '2306.03506'
    at_pub_source_title: Subgraph Networks Based Contrastive Learning
    at_pub_source_date_iso: '2023-06-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.614
    true_std: 0.006
    value_gap_source_arxiv: '2306.03506'
    value_gap_source_title: Subgraph Networks Based Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.614
    sort_std: 0.006
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
  - model: AttrMasking
    model_key: attrmasking
    model_plain: AttrMasking
    value: 0.61
    std: 0.007
    paper_value: 0.61
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: pretraingnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.61
    at_pub_std: 0.007
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6121
    true_std: 0.0065
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.0020999999999999908
    has_value_note: false
    value_note: ''
    sort_value: 0.6121
    sort_std: 0.0065
    global_rank: 135
    paper_rank: 143
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRGCL
    model_key: drgcl
    model_plain: DRGCL
    value: 0.611
    std: 0.008
    paper_value: 0.611
    paper_std: 0.008
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: drgcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.611
    true_std: 0.008
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.611
    sort_std: 0.008
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
  - model: DC-GCL
    model_key: dc-gcl
    model_plain: DC-GCL
    value: 0.606
    std: 0.006
    paper_value: 0.606
    paper_std: 0.006
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.606
    true_std: 0.006
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.606
    sort_std: 0.006
    global_rank: 162
    paper_rank: 162
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimGRACE
    model_key: simgrace
    model_plain: SimGRACE
    value: 0.606
    std: 0.01
    paper_value: 0.606
    paper_std: 0.01
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
    feature_source_evidence: The model is initially pre-trained on the ZINC15 dataset
      and subsequently fine-tuned on the above datasets.
    table_ref: Table 3
    source_ref: simgrace
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6059
    at_pub_std: 0.0096
    at_pub_source_arxiv: '2202.02989'
    at_pub_source_title: Graph Self-supervised Learning with Accurate Discrepancy
      Learning
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.606
    true_std: 0.01
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.606
    sort_std: 0.01
    global_rank: 160
    paper_rank: 160
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: No-pretrain
    model_key: no-pretrain
    model_plain: No-pretrain
    value: 0.581
    std: 0.01
    paper_value: 0.581
    paper_std: 0.01
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on SIDER with Scaffold split
    date: Jun 1, 2024
    date_display: Jun 2024
    date_iso: '2024-06-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.572
    at_pub_std: 0.007
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.009000000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.581
    true_std: 0.01
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.581
    sort_std: 0.01
    global_rank: 213
    paper_rank: 213
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
  - *id005
  - *id006
- benchmark: MoleculeNet
  datasets:
  - *id007
  - *id008
  - *id009
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: NCI1
      dataset_slug: nci1
    - dataset: PROTEINS
      dataset_slug: proteins
    - dataset: COLLAB
      dataset_slug: collab
    - dataset: D&D
      dataset_slug: d-d
    - dataset: RDT-B
      dataset_slug: rdt-b
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: BACE
      dataset_slug: bace
    - dataset: ClinTox
      dataset_slug: clintox
    - dataset: SIDER
      dataset_slug: sider
single_proposed_model: DC-GCL
main_figure: /figures/2406.00403/main_figure.jpegoptim.jpg
---

