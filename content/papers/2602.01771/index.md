---
title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural Understanding'
arxiv_id: '2602.01771'
source_url: ''
authors:
- name: Jingyao Wu
  orcid: null
  s2_author_id: '2384357622'
  s2_url: null
- name: Bin Lu
  orcid: null
  s2_author_id: '2064914349'
  s2_url: null
- name: Zijun Di
  orcid: null
  s2_author_id: '2383911468'
  s2_url: null
- name: Xiaoying Gan
  orcid: null
  s2_author_id: '2283029302'
  s2_url: null
- name: Meng Jin
  orcid: null
  s2_author_id: '2290130264'
  s2_url: null
- name: Luoyi Fu
  orcid: null
  s2_author_id: '1922573'
  s2_url: null
- name: Xinbing Wang
  orcid: null
  s2_author_id: '2354127196'
  s2_url: null
- name: Cheng Zhou
  orcid: null
  s2_author_id: '2111168706'
  s2_url: null
published_date: Feb 2, 2026
published_date_iso: '2026-02-02'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Large language models show great potential in unstructured data understanding,
  but still face significant challenges with graphs due to their structural hallucination.
  Existing approaches mainly either verbalize graphs into natural language, which
  leads to excessive token consumption and scattered attention, or transform graphs
  into trainable continuous embeddings (i.e., soft prompt), but exhibit severe misalignment
  with original text tokens. To solve this problem, we propose to incorporate one
  special token <SO$ _k$> to fully represent the tructure f raph within a unified
  token space, facilitating explicit topology input and structural information sharing.
  Specifically, we propose a topology-aware structural tokenizer that maps each graph
  topology into a highly selective single token. Afterwards, we construct a set of
  hybrid structure Question-Answering corpora to align new structural tokens with
  existing text tokens. With this approach, <SO$ _k$> empowers LLMs to understand,
  generate, and reason in a concise and accurate manner. Extensive experiments on
  five graph-level benchmarks demonstrate the superiority of our method, achieving
  a performance improvement of 9.9–41.4\
codebase_url: https://github.com/Jingyao-Wu/SOG
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Llama3-70b zero-shot
- LLaMA3-3B Zero-shot
- LLaMA3-3B Few-shot (Morgan Sim)
- LLaMA3-3B LoRA SFT
- LLaMA3-3B Soft Prompt
- LLaMA3-3B Few-shot (Random)
- LLaMA3 (70B)
- LLaMA3-3B
mrr: 0.0034
adjusted_mrr: 0.0034
mrr_dataset_count: 4
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 4
  total: 9
task_categories:
- graph_classification
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
  - model: gimlet
    model_key: gimlet
    model_plain: gimlet
    value: 0.696
    std: null
    paper_value: 0.696
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: GIMLET
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6957
    at_pub_std: null
    at_pub_source_arxiv: '2306.13089'
    at_pub_source_title: 'gimlet: A Unified Graph-Text Model for Instruction-Based
      Molecule Zero-Shot Learning'
    at_pub_source_date_iso: '2023-05-28'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.696
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.696
    sort_std: null
    global_rank: 276
    paper_rank: 276
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'gimlet: A Unified Graph-Text Model for Instruction-Based
      Molecule Zero-Shot Learning'
    comparison_source_arxiv: '2306.13089'
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B Few-shot (Random)
    model_key: llama3-3b few-shot (random)
    model_plain: LLaMA3-3B Few-shot (Random)
    value: 0.682
    std: 0.175
    paper_value: 0.682
    paper_std: 0.175
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.682
    true_std: 0.175
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.682
    sort_std: 0.175
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
    is_std_outlier: true
  - model: MolCA-GS
    model_key: molca-gs
    model_plain: MolCA-GS
    value: 0.639
    std: null
    paper_value: 0.639
    paper_std: null
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
    source_ref: Graph2Token
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.639
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.639
    sort_std: null
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
  - model: MolCA-S
    model_key: molca-s
    model_plain: MolCA-S
    value: 0.628
    std: null
    paper_value: 0.628
    paper_std: null
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
    source_ref: Graph2Token
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.628
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.628
    sort_std: null
    global_rank: 293
    paper_rank: 293
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPT-4 Zero-shot
    model_key: gpt-4 zero-shot
    model_plain: GPT-4 Zero-shot
    value: 0.625
    std: null
    paper_value: 0.625
    paper_std: null
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
    source_ref: ChemDFM
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.625
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.625
    sort_std: null
    global_rank: 294
    paper_rank: 294
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPF-AttrMasking
    model_key: gpf-attrmasking
    model_plain: GPF-AttrMasking
    value: 0.622
    std: null
    paper_value: 0.622
    paper_std: null
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
    source_ref: Graph2Token
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.622
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.622
    sort_std: null
    global_rank: 295
    paper_rank: 295
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Galactica-120B Zero-shot
    model_key: galactica-120b zero-shot
    model_plain: Galactica-120B Zero-shot
    value: 0.617
    std: null
    paper_value: 0.617
    paper_std: null
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
    source_ref: MolXPT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.617
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.617
    sort_std: null
    global_rank: 297
    paper_rank: 297
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B LoRA SFT
    model_key: llama2-7b lora sft
    model_plain: LLaMA2-7B LoRA SFT
    value: 0.617
    std: 0.027
    paper_value: 0.617
    paper_std: 0.027
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.617
    true_std: 0.027
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.617
    sort_std: 0.027
    global_rank: 298
    paper_rank: 298
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Few-shot (Morgan Sim)
    model_key: llama2-7b few-shot (morgan sim)
    model_plain: LLaMA2-7B Few-shot (Morgan Sim)
    value: 0.532
    std: 0.015
    paper_value: 0.532
    paper_std: 0.015
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.532
    true_std: 0.015
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.532
    sort_std: 0.015
    global_rank: 310
    paper_rank: 310
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B Zero-shot
    model_key: llama3-3b zero-shot
    model_plain: LLaMA3-3B Zero-shot
    value: 0.527
    std: 0.018
    paper_value: 0.527
    paper_std: 0.018
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.527
    true_std: 0.018
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.527
    sort_std: 0.018
    global_rank: 312
    paper_rank: 312
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Deepseek-R1 Zero-shot
    model_key: deepseek-r1 zero-shot
    model_plain: Deepseek-R1 Zero-shot
    value: 0.527
    std: null
    paper_value: 0.527
    paper_std: null
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
    source_ref: ChemHTS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.527
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.527
    sort_std: null
    global_rank: 311
    paper_rank: 311
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPF-GCL
    model_key: gpf-gcl
    model_plain: GPF-GCL
    value: 0.521
    std: null
    paper_value: 0.521
    paper_std: null
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
    source_ref: Graph2Token
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.521
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.521
    sort_std: null
    global_rank: 313
    paper_rank: 313
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Llama3-70b zero-shot
    model_key: llama3-70b zero-shot
    model_plain: Llama3-70b zero-shot
    value: 0.509
    std: null
    paper_value: 0.509
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ChemHTS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.509
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.509
    sort_std: null
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
  - model: LLaMA3-3B LoRA SFT
    model_key: llama3-3b lora sft
    model_plain: LLaMA3-3B LoRA SFT
    value: 0.505
    std: 0.029
    paper_value: 0.505
    paper_std: 0.029
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.505
    true_std: 0.029
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.505
    sort_std: 0.029
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
  - model: LLaMA2-7B Zero-shot
    model_key: llama2-7b zero-shot
    model_plain: LLaMA2-7B Zero-shot
    value: 0.499
    std: 0.004
    paper_value: 0.499
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.499
    true_std: 0.004
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.499
    sort_std: 0.004
    global_rank: 318
    paper_rank: 318
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Soft Prompt
    model_key: llama2-7b soft prompt
    model_plain: LLaMA2-7B Soft Prompt
    value: 0.494
    std: 0.023
    paper_value: 0.494
    paper_std: 0.023
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.494
    true_std: 0.023
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.494
    sort_std: 0.023
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
  - model: GPT-4o Zero-shot
    model_key: gpt-4o zero-shot
    model_plain: GPT-4o Zero-shot
    value: 0.385
    std: null
    paper_value: 0.385
    paper_std: null
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
    source_ref: ChemHTS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.385
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.385
    sort_std: null
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
  - model: LLaMA3-3B Soft Prompt
    model_key: llama3-3b soft prompt
    model_plain: LLaMA3-3B Soft Prompt
    value: 0.285
    std: 0.009
    paper_value: 0.285
    paper_std: 0.009
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.285
    true_std: 0.009
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.285
    sort_std: 0.009
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
  - model: Galactica-120B Zero-shot
    model_key: galactica-120b zero-shot
    model_plain: Galactica-120B Zero-shot
    value: 0.661
    std: null
    paper_value: 0.661
    paper_std: null
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
    source_ref: MolXPT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.661
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.661
    sort_std: null
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
  - model: Deepseek-R1 Zero-shot
    model_key: deepseek-r1 zero-shot
    model_plain: Deepseek-R1 Zero-shot
    value: 0.636
    std: null
    paper_value: 0.636
    paper_std: null
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
    source_ref: ChemHTS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.636
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.636
    sort_std: null
    global_rank: 276
    paper_rank: 276
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolCA-GS
    model_key: molca-gs
    model_plain: MolCA-GS
    value: 0.636
    std: null
    paper_value: 0.636
    paper_std: null
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
    source_ref: Graph2Token
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.636
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.636
    sort_std: null
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
  - model: MolCA-S
    model_key: molca-s
    model_plain: MolCA-S
    value: 0.625
    std: null
    paper_value: 0.625
    paper_std: null
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
    source_ref: Graph2Token
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.625
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.625
    sort_std: null
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
  - model: GPT-4 Zero-shot
    model_key: gpt-4 zero-shot
    model_plain: GPT-4 Zero-shot
    value: 0.615
    std: null
    paper_value: 0.615
    paper_std: null
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
    source_ref: ChemDFM
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.615
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.615
    sort_std: null
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
  - model: LLaMA3-3B LoRA SFT
    model_key: llama3-3b lora sft
    model_plain: LLaMA3-3B LoRA SFT
    value: 0.602
    std: 0.012
    paper_value: 0.602
    paper_std: 0.012
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.602
    true_std: 0.012
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.602
    sort_std: 0.012
    global_rank: 294
    paper_rank: 294
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Llama3-70b zero-shot
    model_key: llama3-70b zero-shot
    model_plain: Llama3-70b zero-shot
    value: 0.601
    std: null
    paper_value: 0.601
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ChemHTS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.601
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.601
    sort_std: null
    global_rank: 296
    paper_rank: 296
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: gimlet
    model_key: gimlet
    model_plain: gimlet
    value: 0.594
    std: null
    paper_value: 0.594
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: GIMLET
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5939
    at_pub_std: null
    at_pub_source_arxiv: '2306.13089'
    at_pub_source_title: 'gimlet: A Unified Graph-Text Model for Instruction-Based
      Molecule Zero-Shot Learning'
    at_pub_source_date_iso: '2023-05-28'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.594
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.594
    sort_std: null
    global_rank: 298
    paper_rank: 298
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'gimlet: A Unified Graph-Text Model for Instruction-Based
      Molecule Zero-Shot Learning'
    comparison_source_arxiv: '2306.13089'
    is_best: false
    is_std_outlier: false
  - model: GPF-AttrMasking
    model_key: gpf-attrmasking
    model_plain: GPF-AttrMasking
    value: 0.588
    std: null
    paper_value: 0.588
    paper_std: null
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
    source_ref: Graph2Token
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.588
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.588
    sort_std: null
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
  - model: GPT-4o Zero-shot
    model_key: gpt-4o zero-shot
    model_plain: GPT-4o Zero-shot
    value: 0.57
    std: null
    paper_value: 0.57
    paper_std: null
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
    source_ref: ChemHTS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.57
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.57
    sort_std: null
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
  - model: GPF-GCL
    model_key: gpf-gcl
    model_plain: GPF-GCL
    value: 0.565
    std: null
    paper_value: 0.565
    paper_std: null
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
    source_ref: Graph2Token
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.565
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.565
    sort_std: null
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
  - model: LLaMA2-7B LoRA SFT
    model_key: llama2-7b lora sft
    model_plain: LLaMA2-7B LoRA SFT
    value: 0.55
    std: 0.008
    paper_value: 0.55
    paper_std: 0.008
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.55
    true_std: 0.008
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.55
    sort_std: 0.008
    global_rank: 305
    paper_rank: 305
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Soft Prompt
    model_key: llama2-7b soft prompt
    model_plain: LLaMA2-7B Soft Prompt
    value: 0.537
    std: 0.008
    paper_value: 0.537
    paper_std: 0.008
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.537
    true_std: 0.008
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.537
    sort_std: 0.008
    global_rank: 309
    paper_rank: 309
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Few-shot (Morgan Sim)
    model_key: llama2-7b few-shot (morgan sim)
    model_plain: LLaMA2-7B Few-shot (Morgan Sim)
    value: 0.513
    std: 0.008
    paper_value: 0.513
    paper_std: 0.008
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.513
    true_std: 0.008
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.513
    sort_std: 0.008
    global_rank: 310
    paper_rank: 310
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B Zero-shot
    model_key: llama3-3b zero-shot
    model_plain: LLaMA3-3B Zero-shot
    value: 0.502
    std: 0.034
    paper_value: 0.502
    paper_std: 0.034
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.502
    true_std: 0.034
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.502
    sort_std: 0.034
    global_rank: 312
    paper_rank: 312
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Zero-shot
    model_key: llama2-7b zero-shot
    model_plain: LLaMA2-7B Zero-shot
    value: 0.5
    std: 0.0
    paper_value: 0.5
    paper_std: 0.0
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5
    true_std: 0.0
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5
    sort_std: 0.0
    global_rank: 313
    paper_rank: 313
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B Few-shot (Morgan Sim)
    model_key: llama3-3b few-shot (morgan sim)
    model_plain: LLaMA3-3B Few-shot (Morgan Sim)
    value: 0.497
    std: 0.025
    paper_value: 0.497
    paper_std: 0.025
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.497
    true_std: 0.025
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.497
    sort_std: 0.025
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
  - model: LLaMA3-3B Soft Prompt
    model_key: llama3-3b soft prompt
    model_plain: LLaMA3-3B Soft Prompt
    value: 0.279
    std: 0.017
    paper_value: 0.279
    paper_std: 0.017
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.279
    true_std: 0.017
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.279
    sort_std: 0.017
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
  - model: Galactica-120B Zero-shot
    model_key: galactica-120b zero-shot
    model_plain: Galactica-120B Zero-shot
    value: 0.826
    std: null
    paper_value: 0.826
    paper_std: null
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
    source_ref: MolXPT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.826
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.826
    sort_std: null
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B LoRA SFT
    model_key: llama3-3b lora sft
    model_plain: LLaMA3-3B LoRA SFT
    value: 0.638
    std: 0.028
    paper_value: 0.638
    paper_std: 0.028
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.638
    true_std: 0.028
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.638
    sort_std: 0.028
    global_rank: 208
    paper_rank: 208
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B LoRA SFT
    model_key: llama2-7b lora sft
    model_plain: LLaMA2-7B LoRA SFT
    value: 0.593
    std: 0.037
    paper_value: 0.593
    paper_std: 0.037
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.593
    true_std: 0.037
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.593
    sort_std: 0.037
    global_rank: 224
    paper_rank: 224
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B Few-shot (Random)
    model_key: llama3-3b few-shot (random)
    model_plain: LLaMA3-3B Few-shot (Random)
    value: 0.578
    std: 0.062
    paper_value: 0.578
    paper_std: 0.062
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.578
    true_std: 0.062
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.578
    sort_std: 0.062
    global_rank: 232
    paper_rank: 232
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Few-shot (Morgan Sim)
    model_key: llama2-7b few-shot (morgan sim)
    model_plain: LLaMA2-7B Few-shot (Morgan Sim)
    value: 0.568
    std: 0.063
    paper_value: 0.568
    paper_std: 0.063
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.568
    true_std: 0.063
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.568
    sort_std: 0.063
    global_rank: 234
    paper_rank: 234
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPT-4o Zero-shot
    model_key: gpt-4o zero-shot
    model_plain: GPT-4o Zero-shot
    value: 0.518
    std: null
    paper_value: 0.518
    paper_std: null
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
    source_ref: ChemHTS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.518
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.518
    sort_std: null
    global_rank: 241
    paper_rank: 241
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPT-4 Zero-shot
    model_key: gpt-4 zero-shot
    model_plain: GPT-4 Zero-shot
    value: 0.516
    std: null
    paper_value: 0.516
    paper_std: null
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
    source_ref: ChemDFM
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.516
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.516
    sort_std: null
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
  - model: LLaMA3-3B Zero-shot
    model_key: llama3-3b zero-shot
    model_plain: LLaMA3-3B Zero-shot
    value: 0.502
    std: 0.025
    paper_value: 0.502
    paper_std: 0.025
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.502
    true_std: 0.025
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.502
    sort_std: 0.025
    global_rank: 243
    paper_rank: 243
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Soft Prompt
    model_key: llama2-7b soft prompt
    model_plain: LLaMA2-7B Soft Prompt
    value: 0.497
    std: 0.047
    paper_value: 0.497
    paper_std: 0.047
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.497
    true_std: 0.047
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.497
    sort_std: 0.047
    global_rank: 244
    paper_rank: 244
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Llama3-70b zero-shot
    model_key: llama3-70b zero-shot
    model_plain: Llama3-70b zero-shot
    value: 0.488
    std: null
    paper_value: 0.488
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ChemHTS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.488
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.488
    sort_std: null
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
  - model: Deepseek-R1 Zero-shot
    model_key: deepseek-r1 zero-shot
    model_plain: Deepseek-R1 Zero-shot
    value: 0.482
    std: null
    paper_value: 0.482
    paper_std: null
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
    source_ref: ChemHTS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.482
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.482
    sort_std: null
    global_rank: 246
    paper_rank: 246
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Zero-shot
    model_key: llama2-7b zero-shot
    model_plain: LLaMA2-7B Zero-shot
    value: 0.44
    std: 0.026
    paper_value: 0.44
    paper_std: 0.026
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.44
    true_std: 0.026
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.44
    sort_std: 0.026
    global_rank: 247
    paper_rank: 247
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B Soft Prompt
    model_key: llama3-3b soft prompt
    model_plain: LLaMA3-3B Soft Prompt
    value: 0.35
    std: 0.02
    paper_value: 0.35
    paper_std: 0.02
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using AUC-ROC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.35
    true_std: 0.02
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.35
    sort_std: 0.02
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
  - model: Galactica-120B Zero-shot
    model_key: galactica-120b zero-shot
    model_plain: Galactica-120B Zero-shot
    value: 0.689
    std: null
    paper_value: 0.689
    paper_std: null
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.689
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.689
    sort_std: null
    global_rank: 304
    paper_rank: 304
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MolCA-GS
    model_key: molca-gs
    model_plain: MolCA-GS
    value: 0.685
    std: null
    paper_value: 0.685
    paper_std: null
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.685
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.685
    sort_std: null
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
  - model: MolCA-S
    model_key: molca-s
    model_plain: MolCA-S
    value: 0.666
    std: null
    paper_value: 0.666
    paper_std: null
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.666
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.666
    sort_std: null
    global_rank: 311
    paper_rank: 311
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPF-AttrMasking
    model_key: gpf-attrmasking
    model_plain: GPF-AttrMasking
    value: 0.66
    std: null
    paper_value: 0.66
    paper_std: null
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.66
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.66
    sort_std: null
    global_rank: 312
    paper_rank: 312
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPF-GCL
    model_key: gpf-gcl
    model_plain: GPF-GCL
    value: 0.636
    std: null
    paper_value: 0.636
    paper_std: null
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.636
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.636
    sort_std: null
    global_rank: 331
    paper_rank: 331
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: gimlet
    model_key: gimlet
    model_plain: gimlet
    value: 0.612
    std: null
    paper_value: 0.612
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6119
    at_pub_std: null
    at_pub_source_arxiv: '2306.13089'
    at_pub_source_title: 'gimlet: A Unified Graph-Text Model for Instruction-Based
      Molecule Zero-Shot Learning'
    at_pub_source_date_iso: '2023-05-28'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.612
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.612
    sort_std: null
    global_rank: 338
    paper_rank: 338
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'gimlet: A Unified Graph-Text Model for Instruction-Based
      Molecule Zero-Shot Learning'
    comparison_source_arxiv: '2306.13089'
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B LoRA SFT
    model_key: llama2-7b lora sft
    model_plain: LLaMA2-7B LoRA SFT
    value: 0.606
    std: 0.034
    paper_value: 0.606
    paper_std: 0.034
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.606
    true_std: 0.034
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.606
    sort_std: 0.034
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
  - model: Deepseek-R1 Zero-shot
    model_key: deepseek-r1 zero-shot
    model_plain: Deepseek-R1 Zero-shot
    value: 0.601
    std: null
    paper_value: 0.601
    paper_std: null
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.601
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.601
    sort_std: null
    global_rank: 340
    paper_rank: 340
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPT-4 Zero-shot
    model_key: gpt-4 zero-shot
    model_plain: GPT-4 Zero-shot
    value: 0.552
    std: null
    paper_value: 0.552
    paper_std: null
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.552
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.552
    sort_std: null
    global_rank: 344
    paper_rank: 344
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Few-shot (Morgan Sim)
    model_key: llama2-7b few-shot (morgan sim)
    model_plain: LLaMA2-7B Few-shot (Morgan Sim)
    value: 0.511
    std: 0.025
    paper_value: 0.511
    paper_std: 0.025
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.511
    true_std: 0.025
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.511
    sort_std: 0.025
    global_rank: 345
    paper_rank: 345
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B Few-shot (Morgan Sim)
    model_key: llama3-3b few-shot (morgan sim)
    model_plain: LLaMA3-3B Few-shot (Morgan Sim)
    value: 0.51
    std: 0.087
    paper_value: 0.51
    paper_std: 0.087
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.51
    true_std: 0.087
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.51
    sort_std: 0.087
    global_rank: 346
    paper_rank: 346
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B LoRA SFT
    model_key: llama3-3b lora sft
    model_plain: LLaMA3-3B LoRA SFT
    value: 0.508
    std: 0.008
    paper_value: 0.508
    paper_std: 0.008
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.508
    true_std: 0.008
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.508
    sort_std: 0.008
    global_rank: 347
    paper_rank: 347
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Soft Prompt
    model_key: llama2-7b soft prompt
    model_plain: LLaMA2-7B Soft Prompt
    value: 0.498
    std: 0.015
    paper_value: 0.498
    paper_std: 0.015
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.498
    true_std: 0.015
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.498
    sort_std: 0.015
    global_rank: 348
    paper_rank: 348
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B Zero-shot
    model_key: llama3-3b zero-shot
    model_plain: LLaMA3-3B Zero-shot
    value: 0.485
    std: 0.027
    paper_value: 0.485
    paper_std: 0.027
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.485
    true_std: 0.027
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.485
    sort_std: 0.027
    global_rank: 352
    paper_rank: 352
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA2-7B Zero-shot
    model_key: llama2-7b zero-shot
    model_plain: LLaMA2-7B Zero-shot
    value: 0.484
    std: 0.033
    paper_value: 0.484
    paper_std: 0.033
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.484
    true_std: 0.033
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.484
    sort_std: 0.033
    global_rank: 353
    paper_rank: 353
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Llama3-70b zero-shot
    model_key: llama3-70b zero-shot
    model_plain: Llama3-70b zero-shot
    value: 0.449
    std: null
    paper_value: 0.449
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.449
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.449
    sort_std: null
    global_rank: 354
    paper_rank: 354
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3-3B Soft Prompt
    model_key: llama3-3b soft prompt
    model_plain: LLaMA3-3B Soft Prompt
    value: 0.399
    std: 0.019
    paper_value: 0.399
    paper_std: 0.019
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.399
    true_std: 0.019
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.399
    sort_std: 0.019
    global_rank: 355
    paper_rank: 355
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPT-4o Zero-shot
    model_key: gpt-4o zero-shot
    model_plain: GPT-4o Zero-shot
    value: 0.36
    std: null
    paper_value: 0.36
    paper_std: null
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
    protocol_note: Binary graph classification task using ROC-AUC
    date: Feb 2, 2026
    date_display: Feb 2026
    date_iso: '2026-02-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.36
    true_std: null
    value_gap_source_arxiv: '2602.01771'
    value_gap_source_title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural
      Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.36
    sort_std: null
    global_rank: 356
    paper_rank: 356
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
main_figure: /figures/2602.01771/main_figure.jpegoptim.jpg
---

