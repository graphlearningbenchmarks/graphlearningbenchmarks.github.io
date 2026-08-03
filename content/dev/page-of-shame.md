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
| Flagged papers | 913 |
| Flagged rows | 11364 |
| Baseline rows | 11136 |
| Best at pub | 7328 |
| Best today only (not best at pub) | 2903 |
| At-pub best ≠ today's best (different source papers) | 7098 |
| At-pub best = today's best (same source paper) | 4266 |

### Today's best source timing

When the **best reported** holder published relative to the viewing paper:

| Timing | Rows |
|---|---:|
| Already known at publication | 5177 |
| Published later (field moved on) | 6187 |
| Same paper | 0 |
| Unknown date | 0 |

### Most affected datasets

| Dataset | Wrong Rows | Best at pub | Best today only | Papers | Models | Worst Rank Δ |
|---|---:|---:|---:|---:|---:|---:|
| Amazon-Photo | 706 | 506 | 145 | 138 | 97 | 579 |
| Cora | 655 | 458 | 178 | 155 | 114 | 873 |
| PubMed | 643 | 443 | 191 | 136 | 98 | 763 |
| CiteSeer | 615 | 437 | 158 | 136 | 107 | 820 |
| Amazon-Computers | 590 | 386 | 179 | 117 | 84 | 536 |
| Texas | 572 | 336 | 118 | 122 | 91 | 543 |
| Actor | 546 | 406 | 91 | 103 | 85 | 390 |
| Cornell | 527 | 353 | 117 | 121 | 89 | 508 |
| NCI1 | 433 | 281 | 87 | 112 | 76 | 570 |
| MUTAG | 366 | 204 | 65 | 128 | 80 | 708 |
| COLLAB | 283 | 197 | 63 | 75 | 57 | 356 |
| Squirrel | 259 | 176 | 68 | 49 | 48 | 254 |
| Coauthor-Physics | 252 | 158 | 70 | 68 | 46 | 248 |
| WikiCS | 245 | 143 | 72 | 51 | 63 | 227 |
| Chameleon | 239 | 175 | 60 | 50 | 49 | 279 |
| BBBP | 210 | 147 | 48 | 46 | 41 | 287 |
| ogbn-products | 203 | 125 | 56 | 69 | 52 | 337 |
| Coauthor-CS | 197 | 124 | 62 | 48 | 31 | 243 |
| Tox21 | 181 | 134 | 37 | 47 | 39 | 321 |
| ToxCast | 156 | 109 | 40 | 34 | 35 | 179 |
| BACE | 152 | 104 | 34 | 42 | 39 | 281 |
| MD17 | 148 | 106 | 19 | 35 | 28 | 50 |
| SIDER | 139 | 70 | 41 | 37 | 37 | 212 |
| PROTEINS | 131 | 65 | 28 | 62 | 37 | 451 |
| DBLP | 127 | 83 | 34 | 27 | 39 | 171 |

### Most affected models

| Model | Wrong Rows | Best at pub | Best today only | Papers | Datasets | Worst Rank Δ |
|---|---:|---:|---:|---:|---:|---:|
| GCN | 1526 | 1123 | 343 | 507 | 78 | 873 |
| GAT | 1080 | 815 | 217 | 350 | 66 | 843 |
| GraphSAGE | 440 | 258 | 133 | 179 | 52 | 740 |
| MLP | 371 | 238 | 123 | 125 | 36 | 587 |
| GIN | 358 | 230 | 66 | 157 | 54 | 736 |
| DGI | 288 | 171 | 111 | 110 | 26 | 804 |
| APPNP | 258 | 184 | 65 | 95 | 19 | 670 |
| GraphCL | 224 | 135 | 33 | 75 | 26 | 742 |
| SGC | 222 | 156 | 63 | 93 | 26 | 675 |
| GPRGNN | 200 | 121 | 63 | 65 | 28 | 714 |
| MVGRL | 190 | 134 | 41 | 80 | 25 | 524 |
| GRACE | 188 | 114 | 56 | 74 | 21 | 708 |
| GCNII | 187 | 121 | 41 | 76 | 21 | 659 |
| H2GCN | 157 | 118 | 33 | 71 | 21 | 735 |
| InfoGraph | 130 | 80 | 17 | 52 | 12 | 245 |
| BGRL | 122 | 84 | 20 | 48 | 23 | 634 |
| JOAO | 118 | 86 | 26 | 33 | 16 | 280 |
| GCA | 116 | 81 | 30 | 45 | 15 | 641 |
| WL | 115 | 98 | 8 | 56 | 6 | 612 |
| FAGCN | 113 | 90 | 16 | 46 | 17 | 529 |
| GAE | 93 | 63 | 19 | 37 | 17 | 500 |
| ContextPred | 92 | 67 | 23 | 22 | 9 | 286 |
| GraphMAE | 90 | 48 | 28 | 33 | 24 | 661 |
| SAGE | 89 | 39 | 43 | 50 | 24 | 624 |
| DeepWalk | 88 | 61 | 25 | 42 | 16 | 340 |


Detailed table: 913 rows (loaded below).


### Flagged Rows


Detailed table: 500 rows (loaded below).


*Today's best source differs from the at-publication best for that model.