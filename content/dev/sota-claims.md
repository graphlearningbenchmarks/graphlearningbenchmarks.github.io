---
title: SOTA Claims
type: dev
description: Extracted SOTA claims and unrestricted claim audit
---

## SOTA Claims

State-of-the-art performance claims extracted from pre-appendix paper prose (not tables or appendix). Section B audits unrestricted claims against at-publication leaderboard data.

**Total claims:** 10
**Unrestricted:** 1
**Restricted:** 7

### All extracted claims

| Paper | Year | Raw quote | Summary | Datasets | Scope | Restrictions | Source | Confidence |
|-------|------|-----------|---------|----------|-------|--------------|--------|------------|
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | Based on the proposed mechanism, we propose a novel HealHGNN, a node-hyperedge bidirectional system, which achieves heterophily-agnostic message passing with... | HealHGNN achieves heterophily-agnostic message passing with linear complexity and superior performance on... | — | unrestricted | — | Introduction | high |
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | Our model achieves competitive performance across all real-world datasets—matching strong baselines on homophilic hypergraphs and delivering clear gains on heterophilic... | HealHGNN matches strong baselines on homophilic datasets and outperforms them on heterophilic... | — | restricted | baseline_subset: performance is compared specifically against homophilic and heterophilic subsets of datasets | Hypergraph Node Classification (RQ1) | high |
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | Notably, on the Senate dataset we outperform the second-best method by 5%. | HealHGNN outperforms the second-best method on the Senate dataset by 5%. | Senate | restricted | baseline_subset: compared to the second-best method | Hypergraph Node Classification (RQ1) | high |
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | However, as the heterophily level increases, our approach demonstrates a significant improvement. | HealHGNN shows significant improvement over baselines as heterophily increases in synthetic hypergraphs. | Synthetic Hypergraph | restricted | data_source: synthetic hypergraphs with varying heterophily levels | Synthetic Hypergraph under Heterophily | high |
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | In contrast, HealHGNN demonstrates consistently strong performance. | HealHGNN shows consistently strong performance on hypergraph transfer tasks. | — | restricted | data_source: hypergraph transfer tasks (HES, HEP, HER, HED) | Hypergraph Transfer (RQ2) | medium |
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | More importantly, on HEP, HER, and HED, where the structures are more complex and the required propagation distance is longer... | HealHGNN outperforms all other models on complex hypergraph transfer tasks (HEP, HER,... | — | restricted | baseline_subset: compared to all other models on specific complex transfer tasks | Hypergraph Transfer (RQ2) | high |
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | In contrast, HealHGNN achieves superior performance while maintaining linear complexity (|V| + |E|). | HealHGNN achieves superior performance on the Long-Range Graph Benchmark (LRGB) with linear... | Peptides-func, Peptides-struct | restricted | data_source: Long-Range Graph Benchmark (LRGB) | Long-Range Graph Benchmark (RQ2) | high |
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | In contrast, HealHGNN achieves superior performance while maintaining linear complexity ( | | + | |). | HealHGNN achieves superior performance with linear complexity. | — | unclear | model_class: compared to methods with higher computational overhead | Neural Network Depth (RQ3) | medium |
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | As discussed previously, the effect of oversmoothing becomes more severe in heterophilic hypergraphs, amplifying the performance gap in favor of... | HealHGNN shows a larger performance advantage in heterophilic hypergraphs due to better... | House, Senate | restricted | data_source: heterophilic hypergraphs | Neural Network Depth (RQ3) | high |
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | 2026 | Extensive experiments across multiple benchmarks demonstrate that HealHGNN consistently improves performance over competitive baselines. | HealHGNN consistently outperforms competitive baselines across multiple benchmarks. | — | unclear | — | Conclusion | high |

### Unrestricted claim audit

Claims with `scope=unrestricted` and no listed restrictions, compared to the best known result on each dataset at the paper's publication date.

| Paper | Claim | Dataset | Paper result | Best at pub | Prior best paper | Gap | Verdict |
|-------|-------|---------|--------------|-------------|------------------|-----|---------|
| [Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger](/papers/2603.00599/) | Based on the proposed mechanism, we propose a novel HealHGNN, a node-hyperedge bidirectional system, which achieves... | — | — | — | — | — | unverifiable (no datasets named in claim) |