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
| Flagged papers | 969 |
| Flagged rows | 12924 |
| Baseline rows | 12664 |
| Best at pub | 8543 |
| Best today only (not best at pub) | 3458 |
| At-pub best ≠ today's best (different source papers) | 7996 |
| At-pub best = today's best (same source paper) | 4928 |

### Today's best source timing

When the **best reported** holder published relative to the viewing paper:

| Timing | Rows |
|---|---:|
| Already known at publication | 5458 |
| Published later (field moved on) | 7466 |
| Same paper | 0 |
| Unknown date | 0 |

### Most affected datasets

| Dataset | Wrong Rows | Best at pub | Best today only | Papers | Models | Worst Rank Δ |
|---|---:|---:|---:|---:|---:|---:|
| PubMed | 840 | 625 | 207 | 169 | 122 | 896 |
| Cora | 809 | 583 | 210 | 184 | 133 | 1066 |
| CiteSeer | 781 | 583 | 183 | 166 | 138 | 948 |
| Actor | 730 | 534 | 141 | 121 | 93 | 485 |
| Amazon-Photo | 688 | 459 | 189 | 134 | 94 | 685 |
| Texas | 638 | 369 | 156 | 128 | 98 | 656 |
| Amazon-Computers | 578 | 356 | 200 | 114 | 82 | 603 |
| Cornell | 540 | 364 | 123 | 122 | 86 | 623 |
| NCI1 | 523 | 326 | 108 | 122 | 78 | 644 |
| MUTAG | 388 | 205 | 68 | 144 | 76 | 804 |
| COLLAB | 301 | 214 | 67 | 80 | 59 | 384 |
| Squirrel | 286 | 195 | 76 | 52 | 49 | 264 |
| Chameleon | 275 | 204 | 69 | 56 | 55 | 314 |
| WikiCS | 265 | 169 | 83 | 50 | 70 | 281 |
| Coauthor-Physics | 257 | 168 | 76 | 67 | 43 | 344 |
| BBBP | 209 | 142 | 52 | 47 | 46 | 270 |
| ogbn-products | 208 | 136 | 65 | 69 | 50 | 384 |
| Coauthor-CS | 197 | 124 | 62 | 48 | 31 | 251 |
| Tox21 | 183 | 139 | 35 | 48 | 41 | 321 |
| MD17 | 167 | 133 | 34 | 35 | 41 | 115 |
| Amazon-ratings | 156 | 98 | 55 | 35 | 28 | 212 |
| PROTEINS | 155 | 74 | 36 | 69 | 44 | 477 |
| BACE | 153 | 102 | 35 | 42 | 40 | 272 |
| DBLP | 150 | 110 | 37 | 29 | 39 | 191 |
| ToxCast | 150 | 110 | 33 | 33 | 34 | 176 |

### Most affected models

| Model | Wrong Rows | Best at pub | Best today only | Papers | Datasets | Worst Rank Δ |
|---|---:|---:|---:|---:|---:|---:|
| GCN | 1760 | 1316 | 382 | 555 | 78 | 1033 |
| GAT | 1162 | 911 | 218 | 376 | 65 | 995 |
| GraphSAGE | 473 | 290 | 131 | 194 | 52 | 869 |
| GIN | 459 | 315 | 93 | 201 | 56 | 811 |
| MLP | 405 | 259 | 137 | 132 | 36 | 683 |
| APPNP | 299 | 227 | 63 | 105 | 23 | 756 |
| DGI | 267 | 149 | 114 | 107 | 26 | 898 |
| SGC | 254 | 191 | 59 | 98 | 23 | 833 |
| GraphCL | 236 | 138 | 42 | 74 | 25 | 860 |
| GCNII | 231 | 141 | 79 | 91 | 20 | 797 |
| GPRGNN | 220 | 145 | 62 | 69 | 26 | 820 |
| H2GCN | 207 | 143 | 45 | 78 | 21 | 815 |
| MVGRL | 204 | 130 | 64 | 80 | 24 | 759 |
| GRACE | 199 | 108 | 80 | 72 | 21 | 838 |
| GatedGCN | 132 | 90 | 42 | 57 | 14 | 195 |
| InfoGraph | 131 | 82 | 16 | 52 | 12 | 236 |
| FAGCN | 128 | 104 | 17 | 48 | 16 | 704 |
| BGRL | 124 | 88 | 19 | 48 | 23 | 750 |
| JOAO | 122 | 91 | 29 | 35 | 16 | 316 |
| WL | 120 | 102 | 9 | 59 | 6 | 685 |
| GCA | 113 | 78 | 30 | 44 | 15 | 708 |
| GloGNN | 106 | 76 | 28 | 43 | 19 | 723 |
| SAGE | 105 | 52 | 48 | 56 | 24 | 829 |
| DeepWalk | 105 | 75 | 30 | 42 | 16 | 649 |
| JKNet | 104 | 84 | 15 | 37 | 14 | 852 |


Detailed table: 969 rows (loaded below).


### Flagged Rows


Detailed table: 500 rows (loaded below).


*Today's best source differs from the at-publication best for that model.