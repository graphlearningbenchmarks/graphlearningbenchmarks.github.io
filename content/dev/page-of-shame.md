---
title: Page of Shame
type: dev
description: Papers whose reported model values disagree with best reported performance
  (today) and at-publication bests
dev_table_json: /data/development/page-of-shame.json
---

## Page of Shame: Papers Using Wrong Model Values

This page lists papers whose reported primary-metric value for a model disagrees with **best reported** performance (today's global best on the leaderboard) by more than the reported std, or differs at all when no std is given.

Each row also compares against the **best known at publication** (best result for that model on or before the viewing paper's publish date). That split matches the paper pages:

- **Best at pub** — reported value was already worse than the best known when the paper came out (fair criticism; red on paper pages).
- **Best today** (surpassed since publication only) — OK vs the at-publication best, but today's leaderboard best is better (orange on paper pages).
- **Best reported performance** — current leaderboard best (used for rank and the green value).

### Summary

| Statistic | Count |
|---|---:|
| Flagged papers | 942 |
| Flagged rows | 12622 |
| Baseline rows | 12375 |
| Best at pub | 8275 |
| Best today only (not best at pub) | 3395 |
| At-pub best ≠ today's best (different source papers) | 7791 |
| At-pub best = today's best (same source paper) | 4831 |

### Today's best source timing

When the **best reported** holder published relative to the viewing paper:

| Timing | Rows |
|---|---:|
| Already known at publication | 5388 |
| Published later (field moved on) | 7234 |
| Same paper | 0 |
| Unknown date | 0 |

### Most affected datasets

| Dataset | Wrong Rows | Best at pub | Best today only | Papers | Models | Worst Rank Δ |
|---|---:|---:|---:|---:|---:|---:|
| PubMed | 912 | 668 | 234 | 174 | 130 | 944 |
| CiteSeer | 817 | 605 | 194 | 168 | 137 | 959 |
| Cora | 783 | 570 | 187 | 177 | 122 | 1004 |
| Actor | 720 | 526 | 143 | 121 | 93 | 484 |
| Amazon-Photo | 660 | 398 | 218 | 128 | 91 | 628 |
| Texas | 615 | 351 | 152 | 122 | 95 | 618 |
| Amazon-Computers | 540 | 319 | 199 | 106 | 78 | 557 |
| Cornell | 534 | 355 | 127 | 119 | 84 | 608 |
| NCI1 | 521 | 322 | 109 | 121 | 78 | 638 |
| MUTAG | 393 | 209 | 68 | 145 | 76 | 815 |
| Squirrel | 316 | 219 | 79 | 55 | 54 | 272 |
| Chameleon | 309 | 230 | 75 | 59 | 65 | 330 |
| COLLAB | 297 | 208 | 69 | 80 | 58 | 351 |
| Coauthor-Physics | 228 | 144 | 71 | 57 | 43 | 298 |
| BBBP | 218 | 154 | 49 | 46 | 45 | 273 |
| WikiCS | 218 | 132 | 72 | 44 | 59 | 266 |
| ogbn-products | 194 | 128 | 59 | 63 | 48 | 352 |
| Tox21 | 189 | 149 | 32 | 46 | 40 | 314 |
| PROTEINS | 184 | 91 | 39 | 77 | 53 | 511 |
| Coauthor-CS | 173 | 105 | 57 | 42 | 27 | 226 |
| MD17 | 163 | 127 | 36 | 35 | 40 | 113 |
| ToxCast | 162 | 119 | 33 | 33 | 35 | 178 |
| BACE | 157 | 106 | 34 | 40 | 39 | 275 |
| SIDER | 153 | 82 | 37 | 38 | 36 | 222 |
| Amazon-ratings | 136 | 82 | 52 | 31 | 26 | 206 |

### Most affected models

| Model | Wrong Rows | Best at pub | Best today only | Papers | Datasets | Worst Rank Δ |
|---|---:|---:|---:|---:|---:|---:|
| GCN | 1707 | 1266 | 379 | 536 | 76 | 972 |
| GAT | 1126 | 875 | 217 | 362 | 66 | 937 |
| GIN | 449 | 301 | 92 | 196 | 55 | 813 |
| GraphSAGE | 436 | 282 | 102 | 185 | 52 | 914 |
| MLP | 407 | 260 | 138 | 130 | 35 | 719 |
| APPNP | 293 | 222 | 62 | 102 | 24 | 777 |
| DGI | 270 | 158 | 108 | 103 | 24 | 895 |
| SGC | 250 | 189 | 58 | 98 | 22 | 848 |
| GraphCL | 237 | 136 | 45 | 71 | 24 | 646 |
| GCNII | 221 | 138 | 73 | 87 | 18 | 787 |
| GRACE | 205 | 113 | 80 | 73 | 21 | 696 |
| H2GCN | 204 | 137 | 47 | 79 | 20 | 825 |
| MVGRL | 199 | 117 | 73 | 76 | 23 | 771 |
| GPRGNN | 196 | 126 | 58 | 65 | 22 | 830 |
| InfoGraph | 136 | 85 | 17 | 53 | 12 | 233 |
| BGRL | 134 | 99 | 15 | 46 | 22 | 726 |
| GatedGCN | 125 | 82 | 43 | 56 | 14 | 185 |
| FAGCN | 124 | 100 | 17 | 47 | 15 | 711 |
| JOAO | 124 | 95 | 27 | 36 | 16 | 311 |
| GCA | 122 | 84 | 31 | 46 | 15 | 723 |
| WL | 122 | 104 | 9 | 59 | 6 | 696 |
| DeepWalk | 108 | 71 | 36 | 42 | 16 | 691 |
| SAGE | 100 | 51 | 43 | 52 | 25 | 802 |
| GAE | 99 | 61 | 27 | 33 | 17 | 570 |
| ContextPred | 98 | 74 | 22 | 24 | 9 | 241 |


Detailed table: 942 rows (loaded below).


### Flagged Rows


Detailed table: 500 rows (loaded below).


*Today's best source differs from the at-publication best for that model.