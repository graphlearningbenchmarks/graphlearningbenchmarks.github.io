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
| Flagged papers | 964 |
| Flagged rows | 12523 |
| Baseline rows | 12277 |
| Best at pub | 8261 |
| Best today only (not best at pub) | 3144 |
| At-pub best ≠ today's best (different source papers) | 7663 |
| At-pub best = today's best (same source paper) | 4860 |

### Today's best source timing

When the **best reported** holder published relative to the viewing paper:

| Timing | Rows |
|---|---:|
| Already known at publication | 5740 |
| Published later (field moved on) | 6783 |
| Same paper | 0 |
| Unknown date | 0 |

### Most affected datasets

| Dataset | Wrong Rows | Best at pub | Best today only | Papers | Models | Worst Rank Δ |
|---|---:|---:|---:|---:|---:|---:|
| PubMed | 842 | 627 | 208 | 169 | 123 | 896 |
| Cora | 810 | 583 | 209 | 185 | 133 | 1025 |
| CiteSeer | 781 | 583 | 182 | 166 | 138 | 948 |
| Actor | 697 | 501 | 132 | 122 | 91 | 442 |
| Amazon-Photo | 673 | 456 | 165 | 134 | 93 | 585 |
| Texas | 598 | 356 | 124 | 125 | 92 | 558 |
| Amazon-Computers | 578 | 354 | 199 | 114 | 82 | 532 |
| Cornell | 538 | 361 | 117 | 121 | 85 | 544 |
| NCI1 | 504 | 326 | 107 | 122 | 78 | 596 |
| MUTAG | 366 | 203 | 64 | 134 | 76 | 754 |
| COLLAB | 298 | 213 | 61 | 79 | 59 | 361 |
| Squirrel | 286 | 195 | 76 | 52 | 49 | 264 |
| Chameleon | 275 | 204 | 69 | 56 | 55 | 313 |
| WikiCS | 253 | 149 | 75 | 52 | 67 | 236 |
| Coauthor-Physics | 234 | 153 | 61 | 65 | 42 | 252 |
| BBBP | 209 | 142 | 52 | 47 | 46 | 264 |
| ogbn-products | 206 | 133 | 56 | 70 | 49 | 355 |
| Coauthor-CS | 197 | 124 | 62 | 48 | 31 | 251 |
| Tox21 | 183 | 139 | 34 | 48 | 41 | 313 |
| PROTEINS | 155 | 74 | 36 | 69 | 44 | 477 |
| BACE | 153 | 102 | 37 | 42 | 40 | 267 |
| ToxCast | 150 | 110 | 33 | 33 | 34 | 172 |
| Amazon-ratings | 149 | 94 | 51 | 35 | 28 | 183 |
| SIDER | 145 | 74 | 42 | 39 | 37 | 219 |
| Roman-empire | 145 | 107 | 33 | 34 | 25 | 170 |

### Most affected models

| Model | Wrong Rows | Best at pub | Best today only | Papers | Datasets | Worst Rank Δ |
|---|---:|---:|---:|---:|---:|---:|
| GCN | 1717 | 1305 | 357 | 546 | 78 | 1025 |
| GAT | 1154 | 904 | 207 | 377 | 64 | 987 |
| GraphSAGE | 469 | 283 | 132 | 193 | 52 | 869 |
| GIN | 462 | 312 | 92 | 203 | 56 | 811 |
| MLP | 391 | 250 | 129 | 128 | 36 | 683 |
| APPNP | 296 | 225 | 60 | 103 | 22 | 756 |
| DGI | 281 | 151 | 125 | 108 | 26 | 898 |
| SGC | 254 | 192 | 58 | 97 | 23 | 833 |
| GraphCL | 225 | 135 | 33 | 74 | 25 | 860 |
| GCNII | 224 | 138 | 63 | 87 | 20 | 792 |
| GPRGNN | 218 | 143 | 60 | 68 | 26 | 820 |
| MVGRL | 197 | 128 | 56 | 79 | 24 | 759 |
| GRACE | 184 | 107 | 59 | 73 | 21 | 832 |
| H2GCN | 181 | 141 | 34 | 75 | 20 | 815 |
| InfoGraph | 131 | 82 | 16 | 52 | 12 | 229 |
| FAGCN | 128 | 104 | 17 | 48 | 16 | 704 |
| GatedGCN | 125 | 83 | 41 | 58 | 15 | 163 |
| BGRL | 124 | 88 | 18 | 48 | 23 | 744 |
| JOAO | 122 | 90 | 26 | 34 | 16 | 287 |
| WL | 120 | 102 | 9 | 59 | 6 | 652 |
| GCA | 113 | 78 | 30 | 44 | 15 | 708 |
| GloGNN | 105 | 73 | 28 | 44 | 19 | 723 |
| JKNet | 104 | 84 | 13 | 36 | 14 | 852 |
| SAGE | 100 | 49 | 43 | 55 | 24 | 825 |
| DeepWalk | 95 | 64 | 29 | 42 | 16 | 649 |


Detailed table: 964 rows (loaded below).


### Flagged Rows


Detailed table: 500 rows (loaded below).


*Today's best source differs from the at-publication best for that model.