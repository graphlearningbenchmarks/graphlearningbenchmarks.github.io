---
title: Statistics Sources & Discrepancies
type: dev
description: Canonical dataset stats vs paper-reported statistics
---

## Statistics Sources & Discrepancies

Canonical dataset statistics from the database (seeded from `config/seed_data.yaml`) compared with structural statistics reported in papers.

**Datasets with observations:** 9
**Total paper observations:** 9
**Mismatched observations:** 0

### CiteSeer

**Canonical (DB / seed_data.yaml):** graphs=1; nodes=3327.0; edges=4732.0; classes=6; avg_degree=2.845; edge_feature_dim=0; edge_feature_type=citation links; no edge attributes; edge_homophily=0.7062; node_feature_dim=3703; node_feature_type=sparse binary bag-of-words paper features; statistic_notes=PyG exposes 9,104 bidirected edge entries; this record stores 4,732 unique undirected citation links

| Paper | Year | Conference | Reported stats | Match |
|-------|------|------------|----------------|-------|
| [2603.00599](/papers/2603.00599/) | 2026 | — | — | pending |

### Congress

**Canonical (DB / seed_data.yaml):** graphs=1; nodes=1718.0; edges=83105.0; classes=2; avg_hyperedge_size=8.656; avg_node_degree=427.237; clique_expansion_homophily=0.555; edge_count_semantics=hyperedges; edge_feature_dim=0; feature_type=synthetic Gaussian features, dimension 100; median_hyperedge_size=5; node_feature_dim=100; statistic_notes=Congress bills/co-sponsorship release: 1,718 nodes and 83,105 hyperedges.

| Paper | Year | Conference | Reported stats | Match |
|-------|------|------------|----------------|-------|
| [2603.00599](/papers/2603.00599/) | 2026 | — | — | pending |

### Cora

**Canonical (DB / seed_data.yaml):** graphs=1; nodes=2708.0; edges=5429.0; classes=7; avg_degree=4.014; edge_feature_dim=0; edge_homophily=0.8252; node_feature_dim=1433

| Paper | Year | Conference | Reported stats | Match |
|-------|------|------------|----------------|-------|
| [2603.00599](/papers/2603.00599/) | 2026 | — | — | pending |

### Cora-CA

**Canonical (DB / seed_data.yaml):** graphs=1; nodes=2708.0; edges=1072.0; classes=7; avg_hyperedge_size=4.277; avg_node_degree=1.693; clique_expansion_homophily=0.803; edge_count_semantics=hyperedges; edge_feature_dim=0; feature_type=bag_of_words; median_hyperedge_size=3; node_feature_dim=1433; statistic_notes=AllSet supplementary table: 2,708 nodes, 1,072 hyperedges, and 1,433-dimensional document features.

| Paper | Year | Conference | Reported stats | Match |
|-------|------|------------|----------------|-------|
| [2603.00599](/papers/2603.00599/) | 2026 | — | — | pending |

### DBLP-CA

**Canonical (DB / seed_data.yaml):** graphs=1; nodes=41302.0; edges=22363.0; classes=6; avg_hyperedge_size=4.452; avg_node_degree=2.411; clique_expansion_homophily=0.869; edge_count_semantics=hyperedges; edge_feature_dim=0; feature_type=bag_of_words; median_hyperedge_size=3; node_feature_dim=1425; statistic_notes=AllSet supplementary table: 41,302 nodes, 22,363 hyperedges, and 1,425-dimensional document features.

| Paper | Year | Conference | Reported stats | Match |
|-------|------|------------|----------------|-------|
| [2603.00599](/papers/2603.00599/) | 2026 | — | — | pending |

### House

**Canonical (DB / seed_data.yaml):** graphs=1; nodes=1290.0; edges=340.0; classes=2; avg_hyperedge_size=34.73; avg_node_degree=9.181; clique_expansion_homophily=0.509; edge_count_semantics=hyperedges; edge_feature_dim=0; feature_type=synthetic Gaussian features, dimension 100; median_hyperedge_size=40; node_feature_dim=100; statistic_notes=House committee hypergraph: 1,290 nodes and 340 hyperedges in AllSet; the raw committee source can contain 341 before deduplication.

| Paper | Year | Conference | Reported stats | Match |
|-------|------|------------|----------------|-------|
| [2603.00599](/papers/2603.00599/) | 2026 | — | — | pending |

### PubMed

**Canonical (DB / seed_data.yaml):** graphs=1; nodes=19717.0; edges=44338.0; classes=3; avg_degree=4.497; edge_feature_dim=0; edge_feature_type=citation links; no edge attributes; edge_homophily=0.7924; node_feature_dim=500; node_feature_type=sparse TF-IDF paper features; statistic_notes=PyG exposes 88,648 bidirected edge entries; this record stores 44,338 unique undirected citation links

| Paper | Year | Conference | Reported stats | Match |
|-------|------|------------|----------------|-------|
| [2603.00599](/papers/2603.00599/) | 2026 | — | — | pending |

### Senate

**Canonical (DB / seed_data.yaml):** graphs=1; nodes=282.0; edges=315.0; classes=2; avg_hyperedge_size=17.168; avg_node_degree=19.177; clique_expansion_homophily=0.498; edge_count_semantics=hyperedges; edge_feature_dim=0; feature_type=synthetic Gaussian features, dimension 100; median_hyperedge_size=19; node_feature_dim=100; statistic_notes=Senate committee hypergraph: 282 nodes and 315 hyperedges; the Cornell source reports mean hyperedge size 17.2.

| Paper | Year | Conference | Reported stats | Match |
|-------|------|------------|----------------|-------|
| [2603.00599](/papers/2603.00599/) | 2026 | — | — | pending |

### Walmart

**Canonical (DB / seed_data.yaml):** graphs=1; nodes=88860.0; edges=69906.0; classes=11; avg_hyperedge_size=6.589; avg_node_degree=5.184; clique_expansion_homophily=0.53; edge_count_semantics=hyperedges; edge_feature_dim=0; feature_type=synthetic Gaussian features, dimension 100; median_hyperedge_size=5; node_feature_dim=100; statistic_notes=Walmart purchase hypergraph: 88,860 products and 69,906 hyperedges in the AllSet release.

| Paper | Year | Conference | Reported stats | Match |
|-------|------|------------|----------------|-------|
| [2603.00599](/papers/2603.00599/) | 2026 | — | — | pending |
